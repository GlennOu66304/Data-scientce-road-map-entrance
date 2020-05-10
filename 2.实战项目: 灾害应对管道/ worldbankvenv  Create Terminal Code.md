### worldbankvenv  Create Terminal Code
```
Last login: Sun May 10 00:42:10 on ttys000
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
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % cd /Users/zhanghuiqiao/web_app
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % touch Procfile
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % pip freeze
click==7.1.2
Flask==1.1.2
gunicorn==20.0.4
itsdangerous==1.1.0
Jinja2==2.11.2
MarkupSafe==1.1.1
numpy==1.18.4
pandas==1.0.3
plotly==4.7.1
python-dateutil==2.8.1
pytz==2020.1
retrying==1.3.3
six==1.14.0
Werkzeug==1.0.1
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % pip freeze > requirements.txt
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % git init
Initialized empty Git repository in /Users/zhanghuiqiao/web_app/.git/
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % git add . 
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % git commit -m 'first commit'
[master (root-commit) 313e8e4] first commit
 19 files changed, 224 insertions(+)
 create mode 100644 .DS_Store
 create mode 100644 Procfile
 create mode 100644 requirements.txt
 create mode 100644 worldbank.py
 create mode 100644 worldbankapp/.DS_Store
 create mode 100644 worldbankapp/__init__.py
 create mode 100644 worldbankapp/__pycache__/__init__.cpython-36.pyc
 create mode 100644 worldbankapp/__pycache__/routes.cpython-36.pyc
 create mode 100644 worldbankapp/routes.py
 create mode 100644 worldbankapp/static/.DS_Store
 create mode 100644 worldbankapp/static/DS_Store
 create mode 100644 worldbankapp/static/img/DS_Store
 create mode 100644 worldbankapp/static/img/githublogo.png
 create mode 100644 worldbankapp/static/img/linkedinlogo.png
 create mode 100644 worldbankapp/templates/.DS_Store
 create mode 100644 worldbankapp/templates/index.html
 create mode 100644 wrangling_scripts/.DS_Store
 create mode 100644 wrangling_scripts/__pycache__/wrangle_data.cpython-36.pyc
 create mode 100644 wrangling_scripts/wrangle_data.py
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % heroku create web_app 
Creating ⬢ web_app... !
 ▸    Name must start with a letter, end with a letter or digit and can only contain lowercase
 ▸    letters, digits, and dashes.
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % heroku create webapp1 
Creating ⬢ webapp1... !
 ▸    Name webapp1 is already taken
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % heroku create webappworldbank
Creating ⬢ webappworldbank... done
https://webappworldbank.herokuapp.com/ | https://git.heroku.com/webappworldbank.git
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % git remote -v 
heroku	https://git.heroku.com/webappworldbank.git (fetch)
heroku	https://git.heroku.com/webappworldbank.git (push)
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % git push heroku master
Enumerating objects: 27, done.
Counting objects: 100% (27/27), done.
Delta compression using up to 4 threads
Compressing objects: 100% (24/24), done.
Writing objects: 100% (27/27), 13.27 KiB | 2.65 MiB/s, done.
Total 27 (delta 5), reused 0 (delta 0)
remote: Compressing source files... done.
remote: Building source:
remote: 
remote: -----> Python app detected
remote: -----> Installing python-3.6.10
remote: -----> Installing pip
remote: -----> Installing SQLite3
remote: -----> Installing requirements with pip
remote:        Collecting click==7.1.2
remote:          Downloading click-7.1.2-py2.py3-none-anywhl (82 kB)
remote:        Collecting Flask==1.1.2
remote:          Downloading Flask-1.1.2-py2.py3-none-any.whl (94 kB)
remote:        Collecting gunicorn==20.0.4
remote:          Downloading gunicorn-20.0.4-py2.py3-none-any.whl (77 kB)
remote:        Collecting itsdangerous==1.1.0
remote:          Downloading itsdangerous-1.1.0-py2.py3-none-any.whl (16 kB)
remote:        Collecting Jinja2==2.11.2
remote:          Downloading Jinja2-2.11.2-py2.py3-none-any.whl (125 kB)
remote:        Collecting MarkupSafe==1.1.1
remote:          Downloading MarkupSafe-1.1.1-cp36-cp36m-manylinux1_x86_64.whl (27 kB)
remote:        Collecting numpy==1.18.4
remote:          Downloading numpy-1.18.4-cp36-cp36m-manylinux1_x86_64.whl (20.2 MB)
remote:        Collecting pandas==1.0.3
remote:          Downloading pandas-1.0.3-cp36-cp36m-manylinux1_x86_64.whl (10.0 MB)
remote:        Collecting plotly==4.7.1
remote:          Downloading plotly-4.7.1-py2.py3-none-any.whl (11.5 MB)
remote:        Collecting python-dateutil==2.8.1
remote:          Downloading python_dateutil-2.8.1-py2.py3-none-any.whl (227 kB)
remote:        Collecting pytz==2020.1
remote:          Downloading pytz-2020.1-py2.py3-none-any.whl (510 kB)
remote:        Collecting retrying==1.3.3
remote:          Downloading retrying-1.3.3.tar.gz (10 kB)
remote:        Collecting six==1.14.0
remote:          Downloading six-1.14.0-py2.py3-none-any.whl (10 kB)
remote:        Collecting Werkzeug==1.0.1
remote:          Downloading Werkzeug-1.0.1-py2.py3-none-any.whl (298 kB)
remote:        Building wheels for collected packages: retrying
remote:          Building wheel for retrying (setup.py): started
remote:          Building wheel for retrying (setup.py): finished with status 'done'
remote:          Created wheel for retrying: filename=retrying-1.3.3-py3-none-any.whl size=11430 sha256=7b5ba689894118abf2fe727fbdf3f466b64acaac011229f5ebb69d66ebb6a277
remote:          Stored in directory: /tmp/pip-ephem-wheel-cache-nb0mv0tc/wheels/ac/cb/8a/b27bf6323e2f4c462dcbf77d70b7c5e7868a7fbe12871770cf
remote:        Successfully built retrying
remote:        Installing collected packages: click, MarkupSafe, Jinja2, Werkzeug, itsdangerous, Flask, gunicorn, numpy, six, python-dateutil, pytz, pandas, retrying, plotly
remote:        Successfully installed Flask-1.1.2 Jinja2-2.11.2 MarkupSafe-1.1.1 Werkzeug-1.0.1 click-7.1.2 gunicorn-20.0.4 itsdangerous-1.1.0 numpy-1.18.4 pandas-1.0.3 plotly-4.7.1 python-dateutil-2.8.1 pytz-2020.1 retrying-1.3.3 six-1.14.0
remote: -----> Discovering process types
remote:        Procfile declares types -> web
remote: 
remote: -----> Compressing...
remote:        Done: 91.6M
remote: -----> Launching...
remote:        Released v3
remote:        https://webappworldbank.herokuapp.com/ deployed to Heroku
remote: 
remote: Verifying deploy... done.
To https://git.heroku.com/webappworldbank.git
 * [new branch]      master -> master
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % 

```

### web_app test code
```
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % source /Users/zhanghuiqiao/worldbankvenv/bin/activate
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % cd /Users/zhanghuiqiao/web_app 
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % heroku logs --tail  

```