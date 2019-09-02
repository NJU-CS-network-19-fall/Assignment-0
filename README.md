# Assignment 0: Getting start
## Due Sep 11, 2019, 11:59PM (GMT+8)
### Part 0 Build your coding environment
You SHOULD already has a coding environment involving `gcc/g++` `python` `python` and be able to link `dynamic lib`. If not, we recommend you using [Ubuntu](https://ubuntu.com/download/desktop) in [virtue](https://www.baidu.com/s?ie=utf-8&f=8&rsv_bp=1&rsv_idx=1&tn=baidu&wd=ubuntu&rsv_pq=8398d0d200a39636&rsv_t=7d3cwHv0lro9uwWvbfXx05J5VhHynVdwMBqvLWjewSaFtmSJFhvXSQ%2F4K74&rqlang=cn&rsv_enter=1&rsv_dl=tb&rsv_sug3=7&rsv_sug1=5&rsv_sug7=101&rsv_sug2=0&inputT=1004&rsv_sug4=1629&rsv_sug=2) or [entity](https://www.baidu.com/s?ie=utf-8&f=8&rsv_bp=1&rsv_idx=1&tn=baidu&wd=ISO%E5%AE%89%E8%A3%85ubuntu&oq=vmware%2520workstation%2520%25E5%25AE%2589%25E8%25A3%2585ubuntu&rsv_pq=a9978c1f00b4bc28&rsv_t=62c7FNYTcktZpV%2FLAJdq8f4uYdsJEQOBznWIV05%2BnZyEdx0vJExlpQRG39I&rqlang=cn&rsv_enter=1&rsv_dl=tb&inputT=32405&rsv_sug3=64&rsv_sug1=44&rsv_sug7=100&rsv_sug2=0&rsv_sug4=34298).

In the following part of this and many next README file, the notation:
+ `$: command line in Ubuntu/Debian Terminal`
+ `#: some commends/description`

After you set up your Ubuntu or Linux system,

`
$ sudo apt-get install cmake g++ git python3-dev qt5-qmake qt5-default python python3
`

(Optional)
I personally recommend [anaconda](https://www.anaconda.com/distribution/#download-section) as the python develop toolkit with [Jupyter Notebook](https://jupyter.org/install).
In the future work we will provide a `.ipynb` file helping you run a real-time Application layer script. So please install anaconda and Jupyter-Notebook in your Ubuntu system.
````
(Optional) the following steps may not work on some computers
TRY to solve them and feel free to contact TAs(TAs: No we are not free, DO it YOURSELF).

$ cd ~/Desktop
$ mkdir temp
$ cd temp

$ wget https://repo.anaconda.com/archive/Anaconda3-2019.07-Linux-x86_64.sh
# Instead of wget you may also download this file manually
# https://www.anaconda.com/distribution/#download-section
# then choose Python3.7 version Linux 64bit x86 installer

$ sudo chmod u+x Anaconda3-2019.07-Linux-x86_64.sh
$ sudo ./Anaconda3-2019.07-Linux-x86_64.sh
# Then follow the Installation step

# You may face challenges how to link Conda in Terminal -> .bashrc or source
# Please google/baidu it and try to solve them YOURSELF
# This will augment your understanding of how your command and terminal works

# reboot your system | $ sudo reboot

(Optional) you should set a individual workspace for your python/conda environment
Something like $ conda create -n your_env_name python=3.7
Then Activate it

# In Base or your_env_name
$ conda install jupyter
$ conda install jupyter notebook
$ conda install python

If you miss the IMPORT you can install them via conda install or pip install
(Claerly the best way is to Google the solution XD)
````
### Part 1 Git and GitHub
How to use git && GitHub:

Register a GitHub account if you haven't.
````
$ git config --global user.name "YOUR-SCREEN-NAME"
$ git config --global user.email YOUR-EMAIL-ADDRESS
````
Feel free to get more [infomation](https://git-scm.com/book/zh/v2)

You will receive your homework link as YOUR_HW_LINK **Please ALERT the DDL**
````
$ cd ~/Desktop/
$ mkdir hw
$ cd hw
$ git clone YOUR_HW_LINK

# Code with FUN!!!
# ONLY KEEP CHANGE IN YOUR ASSIGNMENT-NUMBER FOLDER
# BECAUSE GIT ONLY SUBMIT WHAT'S IN THE FOLDER (.git)

# Once you finished
# In the ASSIGNMENT-NUMBER folder
$ git add -A
$ git commit -m "some words/marks"
$ git push origin master
# maybe need your GitHub account and passwords
````

### Part 2 Mininet

In the first experiment we will use a simulation tool named [Mininet](http://mininet.org/).
Try to [install](http://mininet.org/download/) it on your Ubuntu system.

In the Option 1,
after you open the VM(user name and password are both 'mininet'), you can also install a working GUI consider now is already in 9012.

````
This conmand are typed in the VM
Update:$ sudo apt-get update
Install the lxde desktop environment:$ sudo apt-get install xinit lxde
Install VirtualBox guest additions:$ sudo apt-get install virtualbox-guest-dkms
Restart the VM:$ sudo reboot
Start the GUI using: $ startx
````

Then check the [tutorial](http://mininet.org/walkthrough/) to check if your Installation is correct and complete.
