## Install Windows Subsystem for Linux 
following https://docs.microsoft.com/en-us/windows/wsl/install-win10

### Check version
```
cat /etc/os-release
```
### Run update
```
sudo apt update && upgrade
```
### Install python3
```
sudo apt install python3 python3-pip ipython3
```
### Install virtualenv
```
python3 -m pip install --user virtualenv
```
### Create virtualenv
```
python3 -m virtualenv p362tfgpu
```
### Activate virtual environment
```
source p362tfgpu/bin/activate
```
### Check python version
```
python --version
```
### Install jupyter
```
pip3 install jupyter
```
### Run jupyter
```
jupyter-notebook
```

## Install spinningup on Windows Subsystem for Linux
### Installing OpenMPI
```
sudo apt-get update && sudo apt-get install libopenmpi-dev
```
### Create virtualenv
```
python3 -m virtualenv spinningup
```
### Create projects folder
```
mkdir projects
cd projects
```
### Select windows folder
```
cd /mnt/d/Projects/mytest
```
### Installing Spinning Up
```
git clone https://github.com/openai/spinningup.git
cd spinningup
pip install -e .
```
