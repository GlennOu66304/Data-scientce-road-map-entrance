# first-neural-network
## 1.Enviroment Building:
### Resources:
1. Dataset:Bike Sharing Dataset Data Set
<br>https://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset
<br>2. Intial code:udacity /cn-deep-learning
<br>https://github.com/udacity/cn-deep-learning

### 2.Coding Enviroment Building:
#### 1.Gitzip download the projeci intial file:
<br>Project folds:first-neural-network
<br>https://github.com/udacity/cn-deep-learning/tree/master/first-neural-network
<br>Gitzip
<br>http://kinolien.github.io/gitzip/

#### 2.conda enviroment build to load jupyter book :
1.Create a conda enviroment:
```
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % conda create --name dlnd python=3
Collecting package metadata (current_repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: /Users/zhanghuiqiao/opt/anaconda3/envs/dlnd

  added / updated specs:
    - python=3


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    certifi-2020.4.5.1         |           py38_0         155 KB
    libffi-3.3                 |       h0a44026_1          45 KB
    ncurses-6.2                |       h0a44026_1         749 KB
    openssl-1.1.1g             |       h1de35cc_0         2.2 MB
    pip-20.0.2                 |           py38_1         1.7 MB
    python-3.8.2               |      hf48f09d_13        20.6 MB
    readline-8.0               |       h1de35cc_0         326 KB
    setuptools-46.1.3          |           py38_0         523 KB
    sqlite-3.31.1              |       h5c1f38d_1         2.4 MB
    wheel-0.34.2               |           py38_0          51 KB
    xz-5.2.5                   |       h1de35cc_0         282 KB
    ------------------------------------------------------------
                                           Total:        29.0 MB

The following NEW packages will be INSTALLED:

  ca-certificates    pkgs/main/osx-64::ca-certificates-2020.1.1-0
  certifi            pkgs/main/osx-64::certifi-2020.4.5.1-py38_0
  libcxx             pkgs/main/osx-64::libcxx-4.0.1-hcfea43d_1
  libcxxabi          pkgs/main/osx-64::libcxxabi-4.0.1-hcfea43d_1
  libedit            pkgs/main/osx-64::libedit-3.1.20181209-hb402a30_0
  libffi             pkgs/main/osx-64::libffi-3.3-h0a44026_1
  ncurses            pkgs/main/osx-64::ncurses-6.2-h0a44026_1
  openssl            pkgs/main/osx-64::openssl-1.1.1g-h1de35cc_0
  pip                pkgs/main/osx-64::pip-20.0.2-py38_1
  python             pkgs/main/osx-64::python-3.8.2-hf48f09d_13
  readline           pkgs/main/osx-64::readline-8.0-h1de35cc_0
  setuptools         pkgs/main/osx-64::setuptools-46.1.3-py38_0
  sqlite             pkgs/main/osx-64::sqlite-3.31.1-h5c1f38d_1
  tk                 pkgs/main/osx-64::tk-8.6.8-ha441bb4_0
  wheel              pkgs/main/osx-64::wheel-0.34.2-py38_0
  xz                 pkgs/main/osx-64::xz-5.2.5-h1de35cc_0
  zlib               pkgs/main/osx-64::zlib-1.2.11-h1de35cc_3


Proceed ([y]/n)? y


Downloading and Extracting Packages
libffi-3.3           | 45 KB     | ##################################### | 100% wheel-0.34.2         | 51 KB     | ##################################### | 100% readline-8.0         | 326 KB    | ##################################### | 100% 
ncurses-6.2          | 749 KB    | ##################################### | 100% 
sqlite-3.31.1        | 2.4 MB    | ##################################### | 100% 
openssl-1.1.1g       | 2.2 MB    | ##################################### | 100% 
certifi-2020.4.5.1   | 155 KB    | ##################################### | 100% 
python-3.8.2         | 20.6 MB   | ##################################### | 100% 
setuptools-46.1.3    | 523 KB    | ##################################### | 100% 
xz-5.2.5             | 282 KB    | ##################################### | 100% 
pip-20.0.2           | 1.7 MB    | ##################################### | 100% 
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
#
# To activate this environment, use
#
#     $ conda activate dlnd
#
# To deactivate an active environment, use
#
#     $ conda deactivate

(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ %
```
2. Active the new enviroment:
```
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % source activate dlnd 
```
3. Install the numpy ，matplotlib， pandas ，and jupyter notebook：
```
(dlnd) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % conda install numpy matplotlib pandas jupyter notebook
Collecting package metadata (current_repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: /Users/zhanghuiqiao/opt/anaconda3/envs/dlnd

  added / updated specs:
    - jupyter
    - matplotlib
    - notebook
    - numpy
    - pandas


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    appnope-0.1.0              |           py38_0           8 KB
    backcall-0.1.0             |           py38_0          21 KB
    cycler-0.10.0              |           py38_0          14 KB
    dbus-1.13.14               |       h517e14e_0         451 KB
    entrypoints-0.3            |           py38_0          10 KB
    icu-58.2                   |       h0a44026_3        10.1 MB
    importlib_metadata-1.5.0   |           py38_0          48 KB
    ipykernel-5.1.4            |   py38h39e3cac_0         171 KB
    ipython-7.13.0             |   py38h5ca1d4c_0         981 KB
    ipython_genutils-0.2.0     |           py38_0          39 KB
    jedi-0.17.0                |           py38_0         780 KB
    jsonschema-3.2.0           |           py38_0          96 KB
    jupyter-1.0.0              |           py38_7           7 KB
    jupyter_client-6.1.3       |             py_0          82 KB
    jupyter_core-4.6.3         |           py38_0          75 KB
    kiwisolver-1.2.0           |   py38h04f5b5a_0          55 KB
    libffi-3.2.1               |       h0a44026_6          43 KB
    libiconv-1.16              |       h1de35cc_0         693 KB
    markupsafe-1.1.1           |   py38h1de35cc_0          31 KB
    matplotlib-3.1.3           |           py38_0          21 KB
    matplotlib-base-3.1.3      |   py38h9aa3819_0         4.9 MB
    mistune-0.8.4              |py38h1de35cc_1000          54 KB
    mkl-service-2.3.0          |   py38hfbe908c_0          42 KB
    mkl_fft-1.0.15             |   py38h5e564d8_0         138 KB
    mkl_random-1.1.0           |   py38h6440ff4_0           5 KB
    nbconvert-5.6.1            |           py38_0         453 KB
    notebook-6.0.3             |           py38_0         4.0 MB
    numpy-1.18.1               |   py38h7241aed_0           5 KB
    numpy-base-1.18.1          |   py38h6575580_1         3.9 MB
    pandas-1.0.3               |   py38h6c726b0_0         7.9 MB
    pandocfilters-1.4.2        |           py38_1          13 KB
    parso-0.7.0                |             py_0          72 KB
    pexpect-4.8.0              |           py38_0          82 KB
    pickleshare-0.7.5          |        py38_1000          13 KB
    prompt-toolkit-3.0.4       |             py_0         244 KB
    prompt_toolkit-3.0.4       |                0          11 KB
    ptyprocess-0.6.0           |           py38_0          23 KB
    pygments-2.6.1             |             py_0         654 KB
    pyqt-5.9.2                 |   py38h655552a_2         3.6 MB
    pyrsistent-0.16.0          |   py38h1de35cc_0          91 KB
    python-3.8.2               |       hc70fcce_0        20.8 MB
    pyzmq-18.1.1               |   py38h0a44026_0         405 KB
    qtconsole-4.7.3            |             py_0          94 KB
    send2trash-1.5.0           |           py38_0          17 KB
    sip-4.19.8                 |   py38h0a44026_0         239 KB
    six-1.14.0                 |           py38_0          26 KB
    terminado-0.8.3            |           py38_0          25 KB
    tornado-6.0.4              |   py38h1de35cc_1         602 KB
    traitlets-4.3.3            |           py38_0         138 KB
    webencodings-0.5.1         |           py38_1          20 KB
    widgetsnbextension-3.5.1   |           py38_0         867 KB
    zipp-3.1.0                 |             py_0          13 KB
    ------------------------------------------------------------
                                           Total:        62.9 MB

The following NEW packages will be INSTALLED:

  appnope            pkgs/main/osx-64::appnope-0.1.0-py38_0
  attrs              pkgs/main/noarch::attrs-19.3.0-py_0
  backcall           pkgs/main/osx-64::backcall-0.1.0-py38_0
  blas               pkgs/main/osx-64::blas-1.0-mkl
  bleach             pkgs/main/noarch::bleach-3.1.4-py_0
  cycler             pkgs/main/osx-64::cycler-0.10.0-py38_0
  dbus               pkgs/main/osx-64::dbus-1.13.14-h517e14e_0
  decorator          pkgs/main/noarch::decorator-4.4.2-py_0
  defusedxml         pkgs/main/noarch::defusedxml-0.6.0-py_0
  entrypoints        pkgs/main/osx-64::entrypoints-0.3-py38_0
  expat              pkgs/main/osx-64::expat-2.2.6-h0a44026_0
  freetype           pkgs/main/osx-64::freetype-2.9.1-hb4e5f40_0
  gettext            pkgs/main/osx-64::gettext-0.19.8.1-h15daf44_3
  glib               pkgs/main/osx-64::glib-2.63.1-hd977a24_0
  icu                pkgs/main/osx-64::icu-58.2-h0a44026_3
  importlib_metadata pkgs/main/osx-64::importlib_metadata-1.5.0-py38_0
  intel-openmp       pkgs/main/osx-64::intel-openmp-2019.4-233
  ipykernel          pkgs/main/osx-64::ipykernel-5.1.4-py38h39e3cac_0
  ipython            pkgs/main/osx-64::ipython-7.13.0-py38h5ca1d4c_0
  ipython_genutils   pkgs/main/osx-64::ipython_genutils-0.2.0-py38_0
  ipywidgets         pkgs/main/noarch::ipywidgets-7.5.1-py_0
  jedi               pkgs/main/osx-64::jedi-0.17.0-py38_0
  jinja2             pkgs/main/noarch::jinja2-2.11.2-py_0
  jpeg               pkgs/main/osx-64::jpeg-9b-he5867d9_2
  jsonschema         pkgs/main/osx-64::jsonschema-3.2.0-py38_0
  jupyter            pkgs/main/osx-64::jupyter-1.0.0-py38_7
  jupyter_client     pkgs/main/noarch::jupyter_client-6.1.3-py_0
  jupyter_console    pkgs/main/noarch::jupyter_console-6.1.0-py_0
  jupyter_core       pkgs/main/osx-64::jupyter_core-4.6.3-py38_0
  kiwisolver         pkgs/main/osx-64::kiwisolver-1.2.0-py38h04f5b5a_0
  libgfortran        pkgs/main/osx-64::libgfortran-3.0.1-h93005f0_2
  libiconv           pkgs/main/osx-64::libiconv-1.16-h1de35cc_0
  libpng             pkgs/main/osx-64::libpng-1.6.37-ha441bb4_0
  libsodium          pkgs/main/osx-64::libsodium-1.0.16-h3efe00b_0
  markupsafe         pkgs/main/osx-64::markupsafe-1.1.1-py38h1de35cc_0
  matplotlib         pkgs/main/osx-64::matplotlib-3.1.3-py38_0
  matplotlib-base    pkgs/main/osx-64::matplotlib-base-3.1.3-py38h9aa3819_0
  mistune            pkgs/main/osx-64::mistune-0.8.4-py38h1de35cc_1000
  mkl                pkgs/main/osx-64::mkl-2019.4-233
  mkl-service        pkgs/main/osx-64::mkl-service-2.3.0-py38hfbe908c_0
  mkl_fft            pkgs/main/osx-64::mkl_fft-1.0.15-py38h5e564d8_0
  mkl_random         pkgs/main/osx-64::mkl_random-1.1.0-py38h6440ff4_0
  nbconvert          pkgs/main/osx-64::nbconvert-5.6.1-py38_0
  nbformat           pkgs/main/noarch::nbformat-5.0.4-py_0
  notebook           pkgs/main/osx-64::notebook-6.0.3-py38_0
  numpy              pkgs/main/osx-64::numpy-1.18.1-py38h7241aed_0
  numpy-base         pkgs/main/osx-64::numpy-base-1.18.1-py38h6575580_1
  pandas             pkgs/main/osx-64::pandas-1.0.3-py38h6c726b0_0
  pandoc             pkgs/main/osx-64::pandoc-2.2.3.2-0
  pandocfilters      pkgs/main/osx-64::pandocfilters-1.4.2-py38_1
  parso              pkgs/main/noarch::parso-0.7.0-py_0
  pcre               pkgs/main/osx-64::pcre-8.43-h0a44026_0
  pexpect            pkgs/main/osx-64::pexpect-4.8.0-py38_0
  pickleshare        pkgs/main/osx-64::pickleshare-0.7.5-py38_1000
  prometheus_client  pkgs/main/noarch::prometheus_client-0.7.1-py_0
  prompt-toolkit     pkgs/main/noarch::prompt-toolkit-3.0.4-py_0
  prompt_toolkit     pkgs/main/noarch::prompt_toolkit-3.0.4-0
  ptyprocess         pkgs/main/osx-64::ptyprocess-0.6.0-py38_0
  pygments           pkgs/main/noarch::pygments-2.6.1-py_0
  pyparsing          pkgs/main/noarch::pyparsing-2.4.7-py_0
  pyqt               pkgs/main/osx-64::pyqt-5.9.2-py38h655552a_2
  pyrsistent         pkgs/main/osx-64::pyrsistent-0.16.0-py38h1de35cc_0
  python-dateutil    pkgs/main/noarch::python-dateutil-2.8.1-py_0
  pytz               pkgs/main/noarch::pytz-2020.1-py_0
  pyzmq              pkgs/main/osx-64::pyzmq-18.1.1-py38h0a44026_0
  qt                 pkgs/main/osx-64::qt-5.9.7-h468cd18_1
  qtconsole          pkgs/main/noarch::qtconsole-4.7.3-py_0
  qtpy               pkgs/main/noarch::qtpy-1.9.0-py_0
  send2trash         pkgs/main/osx-64::send2trash-1.5.0-py38_0
  sip                pkgs/main/osx-64::sip-4.19.8-py38h0a44026_0
  six                pkgs/main/osx-64::six-1.14.0-py38_0
  terminado          pkgs/main/osx-64::terminado-0.8.3-py38_0
  testpath           pkgs/main/noarch::testpath-0.4.4-py_0
  tornado            pkgs/main/osx-64::tornado-6.0.4-py38h1de35cc_1
  traitlets          pkgs/main/osx-64::traitlets-4.3.3-py38_0
  wcwidth            pkgs/main/noarch::wcwidth-0.1.9-py_0
  webencodings       pkgs/main/osx-64::webencodings-0.5.1-py38_1
  widgetsnbextension pkgs/main/osx-64::widgetsnbextension-3.5.1-py38_0
  zeromq             pkgs/main/osx-64::zeromq-4.3.1-h0a44026_3
  zipp               pkgs/main/noarch::zipp-3.1.0-py_0

The following packages will be DOWNGRADED:

  libffi                                     3.3-h0a44026_1 --> 3.2.1-h0a44026_6
  python                                  3.8.2-hf48f09d_13 --> 3.8.2-hc70fcce_0


Proceed ([y]/n)? y


Downloading and Extracting Packages
parso-0.7.0          | 72 KB     | ##################################### | 100% 
send2trash-1.5.0     | 17 KB     | ##################################### | 100% 
dbus-1.13.14         | 451 KB    | ##################################### | 100% 
cycler-0.10.0        | 14 KB     | ##################################### | 100% 
pexpect-4.8.0        | 82 KB     | ##################################### | 100% 
mkl_fft-1.0.15       | 138 KB    | ##################################### | 100% 
ipykernel-5.1.4      | 171 KB    | ##################################### | 100% 
widgetsnbextension-3 | 867 KB    | ##################################### | 100% 
mistune-0.8.4        | 54 KB     | ##################################### | 100% 
ipython-7.13.0       | 981 KB    | ##################################### | 100% 
appnope-0.1.0        | 8 KB      | ############################################### | 100% 
traitlets-4.3.3      | 138 KB    | ############################################### | 100% 
pyrsistent-0.16.0    | 91 KB     | ############################################### | 100% 
nbconvert-5.6.1      | 453 KB    | ############################################### | 100% 
jedi-0.17.0          | 780 KB    | ############################################### | 100% 
terminado-0.8.3      | 25 KB     | ############################################### | 100% 
matplotlib-base-3.1. | 4.9 MB    | ############################################### | 100% 
ptyprocess-0.6.0     | 23 KB     | ############################################### | 100% 
markupsafe-1.1.1     | 31 KB     | ############################################### | 100% 
mkl-service-2.3.0    | 42 KB     | ############################################### | 100% 
pandas-1.0.3         | 7.9 MB    | ############################################### | 100% 
libffi-3.2.1         | 43 KB     | ############################################### | 100% 
kiwisolver-1.2.0     | 55 KB     | ############################################### | 100% 
importlib_metadata-1 | 48 KB     | ############################################### | 100% 
numpy-base-1.18.1    | 3.9 MB    | ############################################### | 100% 
icu-58.2             | 10.1 MB   | ############################################### | 100% 
zipp-3.1.0           | 13 KB     | ############################################### | 100% 
webencodings-0.5.1   | 20 KB     | ############################################### | 100% 
pickleshare-0.7.5    | 13 KB     | ############################################### | 100% 
notebook-6.0.3       | 4.0 MB    | ############################################### | 100% 
pyqt-5.9.2           | 3.6 MB    | ############################################### | 100% 
jupyter_core-4.6.3   | 75 KB     | ############################################### | 100% 
prompt_toolkit-3.0.4 | 11 KB     | ############################################### | 100% 
python-3.8.2         | 20.8 MB   | ############################################### | 100% 
matplotlib-3.1.3     | 21 KB     | ############################################### | 100% 
jsonschema-3.2.0     | 96 KB     | ############################################### | 100% 
jupyter-1.0.0        | 7 KB      | ############################################### | 100% 
pyzmq-18.1.1         | 405 KB    | ############################################### | 100% 
pandocfilters-1.4.2  | 13 KB     | ############################################### | 100% 
qtconsole-4.7.3      | 94 KB     | ############################################### | 100% 
six-1.14.0           | 26 KB     | ############################################### | 100% 
mkl_random-1.1.0     | 5 KB      | ############################################### | 100% 
prompt-toolkit-3.0.4 | 244 KB    | ############################################### | 100% 
backcall-0.1.0       | 21 KB     | ############################################### | 100% 
entrypoints-0.3      | 10 KB     | ############################################### | 100% 
tornado-6.0.4        | 602 KB    | ############################################### | 100% 
sip-4.19.8           | 239 KB    | ############################################### | 100% 
pygments-2.6.1       | 654 KB    | ############################################### | 100% 
ipython_genutils-0.2 | 39 KB     | ############################################### | 100% 
jupyter_client-6.1.3 | 82 KB     | ############################################### | 100% 
numpy-1.18.1         | 5 KB      | ############################################### | 100% 
libiconv-1.16        | 693 KB    | ############################################### | 100% 
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
(dlnd) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ %
```
4. Go to your Anaconda software to find dlnd enviroment and launch it to start your project building:
<br>you can also try code below to launch the jupyter book.
```
jupyter notebook Your-first-neural-network.ipynb
```
5.Project building refer:你的第一个神经网络
<br>https://classroom.udacity.com/nanodegrees/nd025-cn/parts/fecc645f-8b1f-4d73-9754-7b7b380f01e8/modules/21f8b76b-60d1-428d-9b8e-ac17e4837359/lessons/4c03fd28-20ca-40e6-89cc-e72ae96141c2/project

