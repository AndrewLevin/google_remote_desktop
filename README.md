# For using Google Remote Desktop on a virtual machine in CERN's Openstack cloud

1) Go to https://openstack.cern.ch/project/instances/.
2) Launch a CC7 x86_64 m2.medium machine.
3) ssh to the machine from lxplus (e.g. [amlevin@lxplus085 ~]$ ssh amlevin@amlevin8)
4) sudo passwd root (then set a password for root)
5) exit
6) ssh to the machine as root (e.g. [amlevin@lxplus085 ~]$ ssh root@amlevin8)
7) mkdir /home/amlevin/
8) sudo /usr/sbin/usermod -d /home/amlevin -s /bin/bash amlevin
9) chown amlevin: /home/amlevin/
10) chmod go-rx /home/amlevin/
11) sudo -u amlevin cp /etc/skel/.bashrc /home/amlevin/
12) sudo -u amlevin cp /etc/skel/.bash_profile /home/amlevin/
13) sudo -u amlevin cp /etc/skel/.bash_logout /home/amlevin/
14) exit
15) ssh to the machine from lxplus (e.g. [amlevin@lxplus085 ~]$ ssh amlevin@amlevin8)
16) sudo yum install emacs
17) sudo yum groupinstall -y "GNOME Desktop"
18) sudo yum install libappindicator-gtk3
19) sudo yum install libXScrnSaver
20) sudo yum install liberation-fonts
21) sudo yum install chrome-remote-desktop
22) sudo chmod +s /usr/lib64/chrome-remote-desktop/user-session
23) echo "exec gnome-session" >& /home/amlevin/.chrome-remote-desktop-session
24) get the latest version of the nomachine rpm for linux x86_64 from https://www.nomachine.com/download/download&id=2
25) install the rpm (e.g. sudo rpm -i nomachine_6.4.6_1_x86_64.rpm)
26) Connect to the machine using NX 
27) Download the Google Chrome rpm from https://www.google.com/chrome/ 
28) sudo rpm -i google-chrome-stable_current_x86_64.rpm
29) Open Chrome, sign in to your google account, go to the Chrome Web Store, and launch the Chrome Remote Desktop app 
