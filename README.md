# google_remote_desktop
For using Google Remote Desktop on a virtual machine in CERN's Openstack cloud

1) Go to https://openstack.cern.ch/project/instances/.
2) Launch a CC7 x86_6 m2.medium machine.
3) sudo yum install emacs
4) sudo yum groupinstall -y "GNOME Desktop"
5) sudo /usr/sbin/usermod -d /home/amlevin -m -s /bin/bash amlevin
6) ssh root@amlevin1.cern.ch; sudo rpm -i /afs/cern.ch/user/a/amlevin/nomachine_6.0.66_2_x86_64.rpm; exit;

