# google_remote_desktop
For using Google Remote Desktop on a virtual machine in CERN's Openstack cloud

1) Go to https://openstack.cern.ch/project/instances/.
2) Launch a CC7 x86_6 m2.medium machine.
3) ssh to the machine from lxplus (e.g. [amlevin@lxplus085 ~]$ ssh amlevin@amlevin8)
4) sudo passwd root (then set a password for root)
5) exit
6) ssh to the machine as root (e.g. [amlevin@lxplus085 ~]$ ssh root@amlevin8)
7) sudo /usr/sbin/usermod -d /home/amlevin -s /bin/bash amlevin
8) exit
9) ssh to the machine from lxplus (e.g. [amlevin@lxplus085 ~]$ ssh amlevin@amlevin8)
10) sudo yum install emacs
11) sudo yum groupinstall -y "GNOME Desktop"
12) sudo yum install libappindicator-gtk3
13) sudo yum install libXScrnSaver
14) sudo yum install chrome-remote-desktop
15) sudo chmod +s /usr/lib64/chrome-remote-desktop/user-session
16) sudo rpm -i /afs/cern.ch/user/a/amlevin/nomachine_6.0.66_2_x86_64.rpm
17) Connect to the machine using NX 
18) Download the Google Chrome rpm from https://www.google.com/chrome/ 
19) sudo rpm -i google-chrome-stable_current_x86_64.rpm
20) Open Chrome, sign in to your google account, and launch the Chrome Remote Desktop app
