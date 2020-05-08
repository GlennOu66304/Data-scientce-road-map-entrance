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






