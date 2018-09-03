# google_remote_desktop
For using Google Remote Desktop on a virtual machine in CERN's Openstack cloud

1) Go to https://openstack.cern.ch/project/instances/.
2) Launch a CC7 x86_6 m2.medium machine.
3) sudo passwd root (then set a password for root)
4) sudo /usr/sbin/usermod -d /home/amlevin -s /bin/bash amlevin (you will need to ssh to the machine as root in order to do this)
5) sudo yum install emacs
6) sudo yum groupinstall -y "GNOME Desktop"
7) sudo yum install libappindicator-gtk3
8) sudo yum install libXScrnSaver
9) sudo yum install chrome-remote-desktop
10) sudo chmod +s /usr/lib64/chrome-remote-desktop/user-session
11) sudo rpm -i /afs/cern.ch/user/a/amlevin/nomachine_6.0.66_2_x86_64.rpm
12) Connect to the machine using NX 
13) Download the Google Chrome rpm from https://www.google.com/chrome/ 
14) sudo rpm -i google-chrome-stable_current_x86_64.rpm
15) Open Chrome, sign in to your google account, and launch the Chrome Remote Desktop app
