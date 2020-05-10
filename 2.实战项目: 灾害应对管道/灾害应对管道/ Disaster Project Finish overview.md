# Disaster Project Finish overview
## Run Python Method:
```
Last login: Sun May 10 14:13:20 on ttys000
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % cd /Users/zhanghuiqiao/web_app
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % pyhton worldbank.py 
zsh: command not found: pyhton
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % python worldbank.py 
 * Serving Flask app "worldbankapp" (lazy loading)
 * Environment: production
   WARNING: This is a development server. Do not use it in a production deployment.
   Use a production WSGI server instead.
 * Debug mode: on
 * Running on http://0.0.0.0:3001/ (Press CTRL+C to quit)
 * Restarting with fsevents reloader
 * Debugger is active!
 * Debugger PIN: 183-234-804
127.0.0.1 - - [10/May/2020 14:15:52] "GET / HTTP/1.1" 500 -
```

## Project Running Code Flask Method:
```
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % source /Users/zhanghuiqiao/worldbankvenv/bin/activate
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % cd /Users/zhanghuiqiao/web_app             
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % export FLASK_APP=worldbank.py 
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % flask run
 * Serving Flask app "worldbank.py"
 * Environment: production
   WARNING: This is a development server. Do not use it in a production deployment.
   Use a production WSGI server instead.
 * Debug mode: off
/Users/zhanghuiqiao/web_app/worldbank.py:2: Warning: Silently ignoring app.run() because the application is run from the flask command line executable.  Consider putting app.run() behind an if __name__ == "__main__" guard to silence this warning.
  app.run(host='0.0.0.0', port=3001, debug=True)
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```


Udacity-Data-Scientist/2.实战项目: 灾害应对管道/lorem-ipsum-demo-master/
<br>https://github.com/GlennOu66304/Udacity-Data-Scientist/tree/master/2.%E5%AE%9E%E6%88%98%E9%A1%B9%E7%9B%AE:%20%E7%81%BE%E5%AE%B3%E5%BA%94%E5%AF%B9%E7%AE%A1%E9%81%93/lorem-ipsum-demo-master

Deploy project will be put in final step(this can be refered in worldbankvenv  Create Terminal Code.md)

Whole process will follow project lorem-ipsum-demo-master
<br>1. first creat a python virtul wnnviroment 
```
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % python3 -m venv worldbankvenv (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % source /Users/zhanghuiqiao/worldbankvenv/bin/activate
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % pip3 install flask pandas plotly gunicorn
Collecting flask
  Using cached https://files.pythonhosted.org/packages/f2/28/2a03252dfb9ebf377f40fba6a7841b47083260bf8bd8e737b0c6952df83f/Flask-1.1.2-py2.py3-none-any.whl
Collecting pandas
  Using cached https://files.pythonhosted.org/packages/ad/1e/96282ff3db30befbbf8012ea69ecb0adc5e1064ef38e912bb8a3e4cfbccf/pandas-1.0.3-cp37-cp37m-macosx_10_9_x86_64.whl
Collecting plotly
  Downloading https://files.pythonhosted.org/packages/d7/78/eb6cbe96c8379c54819592bb228c58ed7386fcc60a55eca7db99432fdf14/plotly-4.7.1-py2.py3-none-any.whl (11.5MB)
     |████████████████████████████████| 11.5MB 26kB/s 
Collecting gunicorn
  Using cached https://files.pythonhosted.org/packages/69/ca/926f7cd3a2014b16870086b2d0fdc84a9e49473c68a8dff8b57f7c156f43/gunicorn-20.0.4-py2.py3-none-any.whl
Collecting Werkzeug>=0.15 (from flask)
  Using cached https://files.pythonhosted.org/packages/cc/94/5f7079a0e00bd6863ef8f1da638721e9da21e5bacee597595b318f71d62e/Werkzeug-1.0.1-py2.py3-none-any.whl
Collecting itsdangerous>=0.24 (from flask)
  Using cached https://files.pythonhosted.org/packages/76/ae/44b03b253d6fade317f32c24d100b3b35c2239807046a4c953c7b89fa49e/itsdangerous-1.1.0-py2.py3-none-any.whl
Collecting Jinja2>=2.10.1 (from flask)
  Using cached https://files.pythonhosted.org/packages/30/9e/f663a2aa66a09d838042ae1a2c5659828bb9b41ea3a6efa20a20fd92b121/Jinja2-2.11.2-py2.py3-none-any.whl
Collecting click>=5.1 (from flask)
  Using cached https://files.pythonhosted.org/packages/d2/3d/fa76db83bf75c4f8d338c2fd15c8d33fdd7ad23a9b5e57eb6c5de26b430e/click-7.1.2-py2.py3-none-any.whl
Collecting numpy>=1.13.3 (from pandas)
  Using cached https://files.pythonhosted.org/packages/64/1e/982848d4e7b57ed06fbaed251a94d592cc59ebba83e454028f33866d4911/numpy-1.18.4-cp37-cp37m-macosx_10_9_x86_64.whl
Collecting python-dateutil>=2.6.1 (from pandas)
  Using cached https://files.pythonhosted.org/packages/d4/70/d60450c3dd48ef87586924207ae8907090de0b306af2bce5d134d78615cb/python_dateutil-2.8.1-py2.py3-none-any.whl
Collecting pytz>=2017.2 (from pandas)
  Using cached https://files.pythonhosted.org/packages/4f/a4/879454d49688e2fad93e59d7d4efda580b783c745fd2ec2a3adf87b0808d/pytz-2020.1-py2.py3-none-any.whl
Collecting six (from plotly)
  Using cached https://files.pythonhosted.org/packages/65/eb/1f97cb97bfc2390a276969c6fae16075da282f5058082d4cb10c6c5c1dba/six-1.14.0-py2.py3-none-any.whl
Collecting retrying>=1.3.3 (from plotly)
Requirement already satisfied: setuptools>=3.0 in ./worldbankvenv/lib/python3.7/site-packages (from gunicorn) (41.2.0)
Collecting MarkupSafe>=0.23 (from Jinja2>=2.10.1->flask)
  Using cached https://files.pythonhosted.org/packages/ce/c6/f000f1af136ef74e4a95e33785921c73595c5390403f102e9b231b065b7a/MarkupSafe-1.1.1-cp37-cp37m-macosx_10_6_intel.whl
Installing collected packages: Werkzeug, itsdangerous, MarkupSafe, Jinja2, click, flask, numpy, six, python-dateutil, pytz, pandas, retrying, plotly, gunicorn
Successfully installed Jinja2-2.11.2 MarkupSafe-1.1.1 Werkzeug-1.0.1 click-7.1.2 flask-1.1.2 gunicorn-20.0.4 itsdangerous-1.1.0 numpy-1.18.4 pandas-1.0.3 plotly-4.7.1 python-dateutil-2.8.1 pytz-2020.1 retrying-1.3.3 six-1.14.0
WARNING: You are using pip version 19.2.3, however version 20.1 is available.
You should consider upgrading via the 'pip install --upgrade pip' command.
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ %
```
Refer:
<br>worldbankvenv  Create Terminal Code.md
<br>Pyhton Flask Enviroment Building:
<br>https://github.com/GlennOu66304/Udacity-Data-Scientist/blob/master/2.%E5%AE%9E%E6%88%98%E9%A1%B9%E7%9B%AE:%20%E7%81%BE%E5%AE%B3%E5%BA%94%E5%AF%B9%E7%AE%A1%E9%81%93/Pyhton%20Flask.md

<br>2. creat a project fold
```

```

<br>3. Utilize Flask to run the python project first
```
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % cd /Users/zhanghuiqiao/myproject/venv 
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro venv % export FLASK_APP=hello.py 
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro venv % flask run  
 * Serving Flask app "hello.py"
 * Environment: production
   WARNING: This is a development server. Do not use it in a production deployment.
   Use a production WSGI server instead.
 * Debug mode: off
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
127.0.0.1 - - [06/May/2020 23:06:50] "GET / HTTP/1.1" 200 -
127.0.0.1 - - [06/May/2020 23:06:55] "GET /favicon.ico HTTP/1.1" 404 -
```
Run Hello World ! in Browser (Make A Minimal Application)
<br>https://github.com/GlennOu66304/Udacity-Data-Scientist/blob/master/2.%E5%AE%9E%E6%88%98%E9%A1%B9%E7%9B%AE:%20%E7%81%BE%E5%AE%B3%E5%BA%94%E5%AF%B9%E7%AE%A1%E9%81%93/Pyhton%20Flask.md

<br>4. deploy the project to herku
<br>lorem-ipsum-demo-master Heroku.
<br>https://github.com/GlennOu66304/Udacity-Data-Scientist/blob/master/2.%E5%AE%9E%E6%88%98%E9%A1%B9%E7%9B%AE:%20%E7%81%BE%E5%AE%B3%E5%BA%94%E5%AF%B9%E7%AE%A1%E9%81%93/lorem-ipsum-demo-master/lorem-ipsum-demo-master%20Heroku.md
<br>World Bank API Data Dashboard
<br>https://github.com/udacity/DSND_Term2/tree/master/lessons/WebDevelopment/AdvancedDataDashboardCode/world_bank_api_dashboard
<br>How I Built a Dashboard with Dash and Plotly after being stuck in Europe’s Worst Coronavirus Outbreak
<br>https://towardsdatascience.com/how-i-built-a-dashboard-with-dash-and-plotly-after-being-stuck-in-europes-worst-coronavirus-dc41aaeeca4b
<br>Python for Finance: Dash by Plotly
<br>https://towardsdatascience.com/python-for-finance-dash-by-plotly-ccf84045b8be
<br>rebeccaebarnes/income-inequality
<br>https://github.com/rebeccaebarnes/income-inequality