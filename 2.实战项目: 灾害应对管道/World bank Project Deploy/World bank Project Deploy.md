# World bank Project Deploy
1.First Creat a "web_app" fold in your Computer directory:
```
mkdir web_app
mv -t web_app data worldbankapp wrangling_scripts worldbank.py
```
Comment:You need to manually move web_app data worldbankapp wrangling_scripts worldbank.py folds and files into if commmads don't 
work

2. Creat a Python virtual enviroment and activate it:
```
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % cd /Users/zhanghuiqiao 
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % conda update python 
Collecting package metadata (current_repodata.json): done
Solving environment: / 

Updating python is constricted by 

anaconda -> requires python==3.7.6=h359304d_2

If you are sure you want an update of your package either try `conda update --all` or install a specific version of the package you want using `conda install <pkg>=<version>`

done

## Package Plan ##

  environment location: /Users/zhanghuiqiao/opt/anaconda3

  added / updated specs:
    - python


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    conda-package-handling-1.6.1|   py37h1de35cc_0         1.3 MB
    ------------------------------------------------------------
                                           Total:         1.3 MB

The following packages will be REMOVED:

  python_abi-3.7-1_cp37m

The following packages will be UPDATED:

  conda-package-han~                   1.6.0-py37h1de35cc_0 --> 1.6.1-py37h1de35cc_0


Proceed ([y]/n)? y


Downloading and Extracting Packages
conda-package-handli | 1.3 MB    | ############################################## | 100% Preparing transaction: done
Verifying transaction: done
Executing transaction: done
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % python3 -m venv worldbankvenv 
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % source /Users/zhanghuiqiao/worldbankvenv/bin/activate
```
3. PIP install flask pandas plotly gunicorn  package:
```
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % pip3 install flask pandas plotly gunicorn 
Collecting flask
  Using cached https://files.pythonhosted.org/packages/f2/28/2a03252dfb9ebf377f40fba6a7841b47083260bf8bd8e737b0c6952df83f/Flask-1.1.2-py2.py3-none-any.whl
Collecting pandas
  Using cached https://files.pythonhosted.org/packages/ad/1e/96282ff3db30befbbf8012ea69ecb0adc5e1064ef38e912bb8a3e4cfbccf/pandas-1.0.3-cp37-cp37m-macosx_10_9_x86_64.whl
Collecting plotly
  Using cached https://files.pythonhosted.org/packages/4e/9b/1597117623f99b16d87f839b66040a5d3c8a61d83264fdad4388e142944b/plotly-4.7.0-py2.py3-none-any.whl
Collecting gunicorn
  Using cached https://files.pythonhosted.org/packages/69/ca/926f7cd3a2014b16870086b2d0fdc84a9e49473c68a8dff8b57f7c156f43/gunicorn-20.0.4-py2.py3-none-any.whl
Collecting itsdangerous>=0.24 (from flask)
  Using cached https://files.pythonhosted.org/packages/76/ae/44b03b253d6fade317f32c24d100b3b35c2239807046a4c953c7b89fa49e/itsdangerous-1.1.0-py2.py3-none-any.whl
Collecting click>=5.1 (from flask)
  Using cached https://files.pythonhosted.org/packages/d2/3d/fa76db83bf75c4f8d338c2fd15c8d33fdd7ad23a9b5e57eb6c5de26b430e/click-7.1.2-py2.py3-none-any.whl
Collecting Jinja2>=2.10.1 (from flask)
  Using cached https://files.pythonhosted.org/packages/30/9e/f663a2aa66a09d838042ae1a2c5659828bb9b41ea3a6efa20a20fd92b121/Jinja2-2.11.2-py2.py3-none-any.whl
Collecting Werkzeug>=0.15 (from flask)
  Using cached https://files.pythonhosted.org/packages/cc/94/5f7079a0e00bd6863ef8f1da638721e9da21e5bacee597595b318f71d62e/Werkzeug-1.0.1-py2.py3-none-any.whl
Collecting pytz>=2017.2 (from pandas)
  Downloading https://files.pythonhosted.org/packages/4f/a4/879454d49688e2fad93e59d7d4efda580b783c745fd2ec2a3adf87b0808d/pytz-2020.1-py2.py3-none-any.whl (510kB)
     |████████████████████████████████| 512kB 40kB/s 
Collecting numpy>=1.13.3 (from pandas)
  Using cached https://files.pythonhosted.org/packages/64/1e/982848d4e7b57ed06fbaed251a94d592cc59ebba83e454028f33866d4911/numpy-1.18.4-cp37-cp37m-macosx_10_9_x86_64.whl
Collecting python-dateutil>=2.6.1 (from pandas)
  Using cached https://files.pythonhosted.org/packages/d4/70/d60450c3dd48ef87586924207ae8907090de0b306af2bce5d134d78615cb/python_dateutil-2.8.1-py2.py3-none-any.whl
Collecting retrying>=1.3.3 (from plotly)
Collecting six (from plotly)
  Using cached https://files.pythonhosted.org/packages/65/eb/1f97cb97bfc2390a276969c6fae16075da282f5058082d4cb10c6c5c1dba/six-1.14.0-py2.py3-none-any.whl
Requirement already satisfied: setuptools>=3.0 in ./worldbankvenv/lib/python3.7/site-packages (from gunicorn) (41.2.0)
Collecting MarkupSafe>=0.23 (from Jinja2>=2.10.1->flask)
  Using cached https://files.pythonhosted.org/packages/ce/c6/f000f1af136ef74e4a95e33785921c73595c5390403f102e9b231b065b7a/MarkupSafe-1.1.1-cp37-cp37m-macosx_10_6_intel.whl
Installing collected packages: itsdangerous, click, MarkupSafe, Jinja2, Werkzeug, flask, pytz, numpy, six, python-dateutil, pandas, retrying, plotly, gunicorn
Successfully installed Jinja2-2.11.2 MarkupSafe-1.1.1 Werkzeug-1.0.1 click-7.1.2 flask-1.1.2 gunicorn-20.0.4 itsdangerous-1.1.0 numpy-1.18.4 pandas-1.0.3 plotly-4.7.0 python-dateutil-2.8.1 pytz-2020.1 retrying-1.3.3 six-1.14.0
WARNING: You are using pip version 19.2.3, however version 20.1 is available.
You should consider upgrading via the 'pip install --upgrade pip' command.
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % 
```
4.Log in heroku:
```
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % heroku login 
heroku: Press any key to open up the browser to login or q to exit: 
Opening browser to https://cli-auth.heroku.com/auth/cli/browser/b769e8a2-f016-4442-87da-905f10ba9554
Logging in... done
Logged in as 1564468177glen@gmail.com
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % 
```
5. Remove the app.run() in worldbank.py file and save it
<br>6. cd web_app make sure that you are under web_app directory
<br>7.Creat and file Procfile by runing below code in terminal and you will see a rocfile file in web_app directory
```
touch Procfile
```
open the rocfile file, and put the code in it:
```
web gunicorn worldbank:app
```
6. in virtual enviroment, Creat a requirements file and load the package:
```
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % source /Users/zhanghuiqiao/worldbankvenv/bin/activate  
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % cd /Users/zhanghuiqiao/web_app  
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % pip3 freeze > requirements.txt 
```
7. Push the code to heroku:
```
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % git init 
Reinitialized existing Git repository in /Users/zhanghuiqiao/web_app/.git/
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % git add .  
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % git commit -m 'first commit'  
[master ffe546a] first commit
 1 file changed, 14 insertions(+), 255 deletions(-)
 rewrite requirements.txt (97%)
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % heroku create dsnd-udacity-webapp-1 
Creating ⬢ dsnd-udacity-webapp-1... !
 ▸    Name dsnd-udacity-webapp-1 is already taken
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % heroku create dsnd-udacity-webapp-2 
Creating ⬢ dsnd-udacity-webapp-2... done
https://dsnd-udacity-webapp-2.herokuapp.com/ | https://git.heroku.com/dsnd-udacity-webapp-2.git
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % git remote -v 
heroku	https://git.heroku.com/dsnd-udacity-webapp-1.git (fetch)
heroku	https://git.heroku.com/dsnd-udacity-webapp-1.git (push)
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % git push heroku master  
Enumerating objects: 34, done.
Counting objects: 100% (34/34), done.
Delta compression using up to 4 threads
Compressing objects: 100% (30/30), done.
Writing objects: 100% (34/34), 277.78 KiB | 4.34 MiB/s, done.
Total 34 (delta 6), reused 0 (delta 0)
remote: Compressing source files... done.
remote: Building source:
remote: 
remote: -----> Python app detected
remote: -----> Installing python-3.6.10
remote: -----> Installing pip
remote: -----> Installing SQLite3
remote: -----> Installing requirements with pip
remote:        Collecting click==7.1.2
remote:          Downloading click-7.1.2-py2.py3-none-any.whl (82 kB)
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
remote:        Collecting plotly==4.7.0
remote:          Downloading plotly-4.7.0-py2.py3-none-any.whl (11.5 MB)
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
remote:          Created wheel for retrying: filename=retrying-1.3.3-py3-none-any.whl size=11430 sha256=0cb1fa9eccaefd59766d17a398b00043db95e703d580d1e30f862db767b62a72
remote:          Stored in directory: /tmp/pip-ephem-wheel-cache-96dezwjy/wheels/ac/cb/8a/b27bf6323e2f4c462dcbf77d70b7c5e7868a7fbe12871770cf
remote:        Successfully built retrying
remote:        Installing collected packages: click, MarkupSafe, Jinja2, Werkzeug, itsdangerous, Flask, gunicorn, numpy, six, python-dateutil, pytz, pandas, retrying, plotly
remote:        Successfully installed Flask-1.1.2 Jinja2-2.11.2 MarkupSafe-1.1.1 Werkzeug-1.0.1 click-7.1.2 gunicorn-20.0.4 itsdangerous-1.1.0 numpy-1.18.4 pandas-1.0.3 plotly-4.7.0 python-dateutil-2.8.1 pytz-2020.1 retrying-1.3.3 six-1.14.0
remote: -----> Discovering process types
remote:        Procfile declares types -> web
remote: 
remote: -----> Compressing...
remote:        Done: 92M
remote: -----> Launching...
remote:        Released v3
remote:        https://dsnd-udacity-webapp-1.herokuapp.com/ deployed to Heroku
remote: 
remote: Verifying deploy... done.
To https://git.heroku.com/dsnd-udacity-webapp-1.git
 * [new branch]      master -> master
(worldbankvenv) (base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro web_app % 
```
部署
<br>https://classroom.udacity.com/nanodegrees/nd025-cn/parts/f3a1a2fe-76b5-4dd0-85c1-114bd1c1a990/modules/d62339d1-ff64-48e1-9fac-b7d3e129c24b/lessons/060b5796-3ac0-44fc-91dc-d8bdd5738975/concepts/94d181ca-4e7c-46c5-971c-fbc9d4a59f2b





