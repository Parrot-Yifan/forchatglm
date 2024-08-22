# forchatglm

sudo apt install -y build-essential zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev libssl-dev libreadline-dev libffi-dev curl libbz2-dev

# 转镜像源
deb http://mirrors.aliyun.com/ubuntu/ focal main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ focal-updates main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ focal-backports main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ focal-security main restricted universe multiverse

# show 配置
sudo docker run --rm --gpus all nvidia/cuda:11.0-base nvidia-smi

# cuda
https://developer.nvidia.com/cuda-toolkit-archive

# cuda install result
[sudo] password for elex: 
===========
= Summary =
===========

Driver:   Not Selected
Toolkit:  Installed in /usr/local/cuda-12.1/

Please make sure that
 -   PATH includes /usr/local/cuda-12.1/bin
 -   LD_LIBRARY_PATH includes /usr/local/cuda-12.1/lib64, or, add /usr/local/cuda-12.1/lib64 to /etc/ld.so.conf and run ldconfig as root

To uninstall the CUDA Toolkit, run cuda-uninstaller in /usr/local/cuda-12.1/bin
***WARNING: Incomplete installation! This installation did not install the CUDA Driver. A driver of version at least 530.00 is required for CUDA 12.1 functionality to work.
To install the driver using this installer, run the following command, replacing <CudaInstaller> with the name of this run file:
    sudo <CudaInstaller>.run --silent --driver

Logfile is /var/log/cuda-installer.log

# driver install log
[INFO]: Setting silent=true
[INFO]: Setting driver=true
[INFO]: Overriding driver check
[INFO]: Driver installation detected by command: apt list --installed | grep -e nvidia-driver-[0-9][0-9][0-9] -e nvidia-[0-9][0-9][0-9]
[INFO]: Checking compiler version...
[INFO]: gcc location: /usr/bin/gcc

[INFO]: gcc version: gcc version 11.4.0 (Ubuntu 11.4.0-1ubuntu1~22.04)

[INFO]: Initializing menu
[INFO]: nvidia-fs.setKOVersion(2.15.1)
[INFO]: Silent install option: skipping toolkit
[INFO]: Silent install option: skipping toolkit
[INFO]: Silent install option: skipping toolkit
[INFO]: Components to install:
[INFO]: Driver
[INFO]: 530.30.02
[INFO]: Executing NVIDIA-Linux-x86_64-530.30.02.run --ui=none --no-questions --accept-license --disable-nouveau --no-cc-version-check --install-libglvnd  2>&1
[INFO]: Finished with code: 256
[ERROR]: Install of driver component failed. Consult the driver log at /var/log/nvidia-installer.log for more details.
[ERROR]: Install of 530.30.02 failed, quitting


