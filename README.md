# U_J_P
$ sudo vi /etc/network/interfaces 
________________________________________________________
iface eth0 inet static 
address 192.168.0.1 
netmask 255.255.255.0 
gateway 192.168.0.254
dns-nameservers 192.168.0.254 8.8.8.8
auto eth0 
_________________________________________________________
wget -q -O - http://pkg.jenkins-ci.org/debian/jenkins-ci.org.key | sudo apt-key add -

sudo sh -c 'echo deb http://pkg.jenkins-ci.org/debian binary/ > /etc/apt/sources.list.d/jenkins.list'

sudo aptitude update

sudo aptitude install jenkins

__________________________________________________________

http://192.168.0.1:8080

/var/lib/jenkins/users/username/config.xml --> #jbcrypt:$2a$10$razd3L1aXndFfBNHO95aj.IVrFydsxkcQCcLmujmFQzll3hcUrY7S

admin/test

service jenkins restart
