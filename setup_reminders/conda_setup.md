root@jupyter-edmundhenley:/home/jovyan# conda init bash
no change     /opt/conda/condabin/conda
no change     /opt/conda/bin/conda
no change     /opt/conda/bin/conda-env
no change     /opt/conda/bin/activate
no change     /opt/conda/bin/deactivate
no change     /opt/conda/etc/profile.d/conda.sh
no change     /opt/conda/etc/fish/conf.d/conda.fish
no change     /opt/conda/shell/condabin/Conda.psm1
no change     /opt/conda/shell/condabin/conda-hook.ps1
no change     /opt/conda/lib/python3.7/site-packages/xontrib/conda.xsh
no change     /opt/conda/etc/profile.d/conda.csh
modified      /root/.bashrc

==> For changes to take effect, close and re-open your current shell. <==

root@jupyter-edmundhenley:/home/jovyan# # Edmund closed and reopened

(base) root@jupyter-edmundhenley:/home/jovyan#  # Got this on reopening

(base) root@jupyter-edmundhenley:/home/jovyan# conda create --name edmund-workshop --yes # don't ask for confirmation
Collecting package metadata (current_repodata.json): done
Solving environment: done


==> WARNING: A newer version of conda exists. <==
  current version: 4.7.10
  latest version: 4.7.12

Please update conda by running

    $ conda update -n base -c defaults conda



## Package Plan ##

  environment location: /root/my-conda-envs/edmund-workshop



Preparing transaction: done
Verifying transaction: done
Executing transaction: done
#
# To activate this environment, use
#
#     $ conda activate edmund-workshop
#
# To deactivate an active environment, use
#
#     $ conda deactivate
(base) root@jupyter-edmundhenley:/home/jovyan# conda activate edmund-workshop

(/root/my-conda-envs/edmund-workshop) root@jupyter-edmundhenley:/home/jovyan# conda install ipykernel --yes
Collecting package metadata (current_repodata.json): done
Solving environment: done


==> WARNING: A newer version of conda exists. <==
  current version: 4.7.10
  latest version: 4.7.12

Please update conda by running

    $ conda update -n base -c defaults conda



## Package Plan ##

  environment location: /root/my-conda-envs/edmund-workshop

  added / updated specs:
    - ipykernel


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    _libgcc_mutex-0.1          |             main           3 KB
    backcall-0.1.0             |           py37_0          20 KB
    ca-certificates-2019.10.16 |                0         131 KB
    certifi-2019.9.11          |           py37_0         154 KB
    decorator-4.4.1            |             py_0          13 KB
    ipykernel-5.1.3            |   py37h39e3cac_0         167 KB
    ipython-7.9.0              |   py37h39e3cac_0         1.1 MB
    ipython_genutils-0.2.0     |           py37_0          39 KB
    jedi-0.15.1                |           py37_0         704 KB
    jupyter_client-5.3.4       |           py37_0         136 KB
    jupyter_core-4.6.1         |           py37_0          74 KB
    libedit-3.1.20181209       |       hc058e9b_0         163 KB
    libffi-3.2.1               |       hd88cf55_4          40 KB
    libgcc-ng-9.1.0            |       hdf63c60_0         5.1 MB
    libsodium-1.0.16           |       h1bed415_0         214 KB
    libstdcxx-ng-9.1.0         |       hdf63c60_0         3.1 MB
    ncurses-6.1                |       he6710b0_1         777 KB
    openssl-1.1.1d             |       h7b6447c_3         3.7 MB
    parso-0.5.1                |             py_0          68 KB
    pexpect-4.7.0              |           py37_0          80 KB
    pickleshare-0.7.5          |           py37_0          13 KB
    pip-19.3.1                 |           py37_0         1.9 MB
    prompt_toolkit-2.0.10      |             py_0         227 KB
    ptyprocess-0.6.0           |           py37_0          23 KB
    pygments-2.4.2             |             py_0         664 KB
    python-3.7.5               |       h0371630_0        32.2 MB
    python-dateutil-2.8.0      |           py37_0         266 KB
    pyzmq-18.1.0               |   py37he6710b0_0         455 KB
    readline-7.0               |       h7b6447c_5         324 KB
    setuptools-41.6.0          |           py37_0         652 KB
    six-1.12.0                 |           py37_0          23 KB
    sqlite-3.30.1              |       h7b6447c_0         1.9 MB
    tk-8.6.8                   |       hbc83047_0         2.8 MB
    tornado-6.0.3              |   py37h7b6447c_0         584 KB
    traitlets-4.3.3            |           py37_0         138 KB
    wcwidth-0.1.7              |           py37_0          22 KB
    wheel-0.33.6               |           py37_0          40 KB
    xz-5.2.4                   |       h14c3975_4         283 KB
    zeromq-4.3.1               |       he6710b0_3         496 KB
    zlib-1.2.11                |       h7b6447c_3         103 KB
    ------------------------------------------------------------
                                           Total:        58.7 MB

The following NEW packages will be INSTALLED:

  _libgcc_mutex      pkgs/main/linux-64::_libgcc_mutex-0.1-main
  backcall           pkgs/main/linux-64::backcall-0.1.0-py37_0
  ca-certificates    pkgs/main/linux-64::ca-certificates-2019.10.16-0
  certifi            pkgs/main/linux-64::certifi-2019.9.11-py37_0
  decorator          pkgs/main/noarch::decorator-4.4.1-py_0
  ipykernel          pkgs/main/linux-64::ipykernel-5.1.3-py37h39e3cac_0
  ipython            pkgs/main/linux-64::ipython-7.9.0-py37h39e3cac_0
  ipython_genutils   pkgs/main/linux-64::ipython_genutils-0.2.0-py37_0
  jedi               pkgs/main/linux-64::jedi-0.15.1-py37_0
  jupyter_client     pkgs/main/linux-64::jupyter_client-5.3.4-py37_0
  jupyter_core       pkgs/main/linux-64::jupyter_core-4.6.1-py37_0
  libedit            pkgs/main/linux-64::libedit-3.1.20181209-hc058e9b_0
  libffi             pkgs/main/linux-64::libffi-3.2.1-hd88cf55_4
  libgcc-ng          pkgs/main/linux-64::libgcc-ng-9.1.0-hdf63c60_0
  libsodium          pkgs/main/linux-64::libsodium-1.0.16-h1bed415_0
  libstdcxx-ng       pkgs/main/linux-64::libstdcxx-ng-9.1.0-hdf63c60_0
  ncurses            pkgs/main/linux-64::ncurses-6.1-he6710b0_1
  openssl            pkgs/main/linux-64::openssl-1.1.1d-h7b6447c_3
  parso              pkgs/main/noarch::parso-0.5.1-py_0
  pexpect            pkgs/main/linux-64::pexpect-4.7.0-py37_0
  pickleshare        pkgs/main/linux-64::pickleshare-0.7.5-py37_0
  pip                pkgs/main/linux-64::pip-19.3.1-py37_0
  prompt_toolkit     pkgs/main/noarch::prompt_toolkit-2.0.10-py_0
  ptyprocess         pkgs/main/linux-64::ptyprocess-0.6.0-py37_0
  pygments           pkgs/main/noarch::pygments-2.4.2-py_0
  python             pkgs/main/linux-64::python-3.7.5-h0371630_0
  python-dateutil    pkgs/main/linux-64::python-dateutil-2.8.0-py37_0
  pyzmq              pkgs/main/linux-64::pyzmq-18.1.0-py37he6710b0_0
  readline           pkgs/main/linux-64::readline-7.0-h7b6447c_5
  setuptools         pkgs/main/linux-64::setuptools-41.6.0-py37_0
  six                pkgs/main/linux-64::six-1.12.0-py37_0
  sqlite             pkgs/main/linux-64::sqlite-3.30.1-h7b6447c_0
  tk                 pkgs/main/linux-64::tk-8.6.8-hbc83047_0
  tornado            pkgs/main/linux-64::tornado-6.0.3-py37h7b6447c_0
  traitlets          pkgs/main/linux-64::traitlets-4.3.3-py37_0
  wcwidth            pkgs/main/linux-64::wcwidth-0.1.7-py37_0
  wheel              pkgs/main/linux-64::wheel-0.33.6-py37_0
  xz                 pkgs/main/linux-64::xz-5.2.4-h14c3975_4
  zeromq             pkgs/main/linux-64::zeromq-4.3.1-he6710b0_3
  zlib               pkgs/main/linux-64::zlib-1.2.11-h7b6447c_3



Downloading and Extracting Packages
libgcc-ng-9.1.0      | 5.1 MB    | ################################################################################## | 100% 
_libgcc_mutex-0.1    | 3 KB      | ################################################################################## | 100% 
ca-certificates-2019 | 131 KB    | ################################################################################## | 100% 
readline-7.0         | 324 KB    | ################################################################################## | 100% 
libffi-3.2.1         | 40 KB     | ################################################################################## | 100% 
python-3.7.5         | 32.2 MB   | ################################################################################## | 100% 
pickleshare-0.7.5    | 13 KB     | ################################################################################## | 100% 
prompt_toolkit-2.0.1 | 227 KB    | ################################################################################## | 100% 
sqlite-3.30.1        | 1.9 MB    | ################################################################################## | 100% 
certifi-2019.9.11    | 154 KB    | ################################################################################## | 100% 
zlib-1.2.11          | 103 KB    | ################################################################################## | 100% 
traitlets-4.3.3      | 138 KB    | ################################################################################## | 100% 
pip-19.3.1           | 1.9 MB    | ################################################################################## | 100% 
zeromq-4.3.1         | 496 KB    | ################################################################################## | 100% 
ipython-7.9.0        | 1.1 MB    | ################################################################################## | 100% 
parso-0.5.1          | 68 KB     | ################################################################################## | 100% 
six-1.12.0           | 23 KB     | ################################################################################## | 100% 
jupyter_client-5.3.4 | 136 KB    | ################################################################################## | 100% 
tornado-6.0.3        | 584 KB    | ################################################################################## | 100% 
python-dateutil-2.8. | 266 KB    | ################################################################################## | 100% 
libstdcxx-ng-9.1.0   | 3.1 MB    | ################################################################################## | 100% 
tk-8.6.8             | 2.8 MB    | ################################################################################## | 100% 
decorator-4.4.1      | 13 KB     | ################################################################################## | 100% 
pyzmq-18.1.0         | 455 KB    | ################################################################################## | 100% 
backcall-0.1.0       | 20 KB     | ################################################################################## | 100% 
libedit-3.1.20181209 | 163 KB    | ################################################################################## | 100% 
ptyprocess-0.6.0     | 23 KB     | ################################################################################## | 100% 
wheel-0.33.6         | 40 KB     | ################################################################################## | 100% 
ipykernel-5.1.3      | 167 KB    | ################################################################################## | 100% 
ncurses-6.1          | 777 KB    | ################################################################################## | 100% 
jedi-0.15.1          | 704 KB    | ################################################################################## | 100% 
ipython_genutils-0.2 | 39 KB     | ################################################################################## | 100% 
libsodium-1.0.16     | 214 KB    | ################################################################################## | 100% 
pexpect-4.7.0        | 80 KB     | ################################################################################## | 100% 
jupyter_core-4.6.1   | 74 KB     | ################################################################################## | 100% 
setuptools-41.6.0    | 652 KB    | ################################################################################## | 100% 
xz-5.2.4             | 283 KB    | ################################################################################## | 100% 
wcwidth-0.1.7        | 22 KB     | ################################################################################## | 100% 
pygments-2.4.2       | 664 KB    | ################################################################################## | 100% 
openssl-1.1.1d       | 3.7 MB    | ################################################################################## | 100% 
Preparing transaction: done
Verifying transaction: done
Executing transaction: done


(/root/my-conda-envs/edmund-workshop) root@jupyter-edmundhenley:/home/jovyan# python -m ipykernel install --name "edmund-workshop" --display-name "EdEnv" --user
Installed kernelspec edmund-workshop in /home/jovyan/.local/share/jupyter/kernels/edmund-workshop
(/root/my-conda-envs/edmund-workshop) root@jupyter-edmundhenley:/home/jovyan#