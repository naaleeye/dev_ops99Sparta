# dev_ops99Sparta

# create a virtual machine with Linux Ubuntu 16.04
# ubuntu/xenial64

Vagrant.configure("2") do |config|

 # choose the os/box/distro
 config.vm.box = "ubuntu/xenial64"
 config.vm.network "private_network", ip: "192.168.56.0/21"
 config.vm.network "forwarded_port", guest: 80, host: 8080

#Vagrant destroy
#Vagrant up
#Vagrant reload

end

Who am I 'uname -a'
Where am I 'pwd'
list dir or all 'ls' or 'ls -a'
copy file 'cp filename destination'
create file 'touch filename'
create folder 'mkdir foldername'
how to navigate 'cd foldername' return step back 'cd ..'
deleting file folder 'rm -rf namefolder'

Task: Create a folder called test, create a file called text.txt inside the test folder then copy the file to your home location 'home/vagrant'

""File Permissions""
- Read 'r', write 'W' and 'X'
- How to check permissions '11'
- change permission 'chmod'permission '' filename

find out all processes running 'top'
how to 'kill' a process 
