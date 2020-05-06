# Pyhton Flask
## Enviroment Building:
1.install Flask:
```
Last login: Wed May  6 21:25:51 on ttys000
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % mkdir myproject 
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % cd myproject 
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro myproject % python3 -m venv venv 
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro myproject % . venv/bin/activate 
(venv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro myproject % pip install Flask
Collecting Flask
  Downloading https://files.pythonhosted.org/packages/f2/28/2a03252dfb9ebf377f40fba6a7841b47083260bf8bd8e737b0c6952df83f/Flask-1.1.2-py2.py3-none-any.whl (94kB)
     |████████████████████████████████| 102kB 18kB/s 
Collecting click>=5.1 (from Flask)
  Downloading https://files.pythonhosted.org/packages/d2/3d/fa76db83bf75c4f8d338c2fd15c8d33fdd7ad23a9b5e57eb6c5de26b430e/click-7.1.2-py2.py3-none-any.whl (82kB)
     |████████████████████████████████| 92kB 15kB/s 
Collecting itsdangerous>=0.24 (from Flask)
  Downloading https://files.pythonhosted.org/packages/76/ae/44b03b253d6fade317f32c24d100b3b35c2239807046a4c953c7b89fa49e/itsdangerous-1.1.0-py2.py3-none-any.whl
Collecting Jinja2>=2.10.1 (from Flask)
  Using cached https://files.pythonhosted.org/packages/30/9e/f663a2aa66a09d838042ae1a2c5659828bb9b41ea3a6efa20a20fd92b121/Jinja2-2.11.2-py2.py3-none-any.whl
Collecting Werkzeug>=0.15 (from Flask)
  Downloading https://files.pythonhosted.org/packages/cc/94/5f7079a0e00bd6863ef8f1da638721e9da21e5bacee597595b318f71d62e/Werkzeug-1.0.1-py2.py3-none-any.whl (298kB)
     |████████████████████████████████| 307kB 9.5kB/s 
Collecting MarkupSafe>=0.23 (from Jinja2>=2.10.1->Flask)
  Downloading https://files.pythonhosted.org/packages/ce/c6/f000f1af136ef74e4a95e33785921c73595c5390403f102e9b231b065b7a/MarkupSafe-1.1.1-cp37-cp37m-macosx_10_6_intel.whl
Installing collected packages: click, itsdangerous, MarkupSafe, Jinja2, Werkzeug, Flask
Successfully installed Flask-1.1.2 Jinja2-2.11.2 MarkupSafe-1.1.1 Werkzeug-1.0.1 click-7.1.2 itsdangerous-1.1.0
WARNING: You are using pip version 19.2.3, however version 20.1 is available.
You should consider upgrading via the 'pip install --upgrade pip' command.
(venv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro myproject % 
```
Installation
<br>https://flask.palletsprojects.com/en/1.1.x/installation/#installation

## Run Hello World ! in Browser (Make A Minimal Application)
<br>open the project"myproject" in pycharm, Find myproject-->venv Then Open it in Pycharm;
<br>creat a hello.py file  the venv fold and seprate from bin,include lib fold.
<br>write the code in hello.py file and save it.
```
from flask import Flask
app = Flask(__name__)

@app.route('/')
def hello_world():
    return 'Hello, World!'
```
<br>creat Link in Terminal:
move to My project direct and write the code below:
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




