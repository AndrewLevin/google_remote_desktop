# google_remote_desktop
For using Google Remote Desktop on a virtual machine in CERN's Openstack cloud

1) Go to https://openstack.cern.ch/project/instances/.
2) Launch a CC7 x86_6 m2.medium machine.
3) sudo yum install emacs
4) sudo yum groupinstall -y "GNOME Desktop"
5) sudo yum install libappindicator-gtk3
6) sudo yum install libXScrnSaver
7) sudo yum install chrome-remote-desktop
8) sudo /usr/sbin/usermod -d /home/amlevin -s /bin/bash amlevin (you will need to ssh to the machine as root in order to do this)
9) sudo rpm -i /afs/cern.ch/user/a/amlevin/nomachine_6.0.66_2_x86_64.rpm
10) Connect to the machine using NX 
11) Download the Google Chrome rpm from https://www.google.com/chrome/ 
12) sudo rpm -i google-chrome-stable_current_x86_64.rpm
13) Open Chrome and sign in to your google account
