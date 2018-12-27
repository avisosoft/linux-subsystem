# Install Windows Subsystem for Linux 
following https://docs.microsoft.com/en-us/windows/wsl/install-win10

### Check version
cat /etc/os-release

### Run update
sudo apt update && upgrade

### Install python3
sudo apt install python3 python3-pip ipython3

### Install virtualenv
python3 -m pip install --user virtualenv

### Create virtualenv
python3 -m virtualenv p362tfgpu

### Activate virtual environment
source p362tfgpu/bin/activate

### Check python version
python --version

### Install jupyter
pip3 install jupyter

### Run jupyter
jupyter-notebook

