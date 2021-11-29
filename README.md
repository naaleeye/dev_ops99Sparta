# DevOps Intro
## Development Env

- Install vagrant
- Install Ruby


**Linux commands**
- `sudo apt-get update -y`
```
# creating a virtual machine with Linux Ubuntu 16.04
# ubuntu/xenial64

Vagrant.configure("2") do |config|

 # choose the os/box/distro
 config.vm.box = "ubuntu/xenial64"
 config.vm.network "private_network", ip: "192.168.10.100"  
# vagrant destroy
# vagrant up
# vagrant reload
end
```

""Linux Commands""
vagrant up Create virtual machine
vagrant destroy Destroy virtual machine
vagrant reload reload virtual machine
systemctl status nginx - check the status of nginx
vagrant ssh - connect to the virtual machine from bash
sudo apt-get update -y
sudo apt-get upgrade -y
sudo apt-get install nginx -y

- Who am I `uname -a`
- Where am I `pwd`
- list dir or all `ls` or `ls -a`
- copy file `cp filename destination`
- cut or rename `mv filename destination`
- create file `touch filename`
- create folder `mkdir foldername`
- how to navigate `cd foldername` retrun step back `cd ..`
- deleting file folders `rm -rf namefolder`

> Task: Create a folder called test, create a file called text.txt inside the test folder then copy the text.txt to your home location `/home/vagrant`

**File Permissions**
- Read `r`, Write `w` and `x`
- how to check permissions `ll`
- change permision `chmod permision filename`

- find out all processes running `top`
- how to `kill` a process 

### Automate everything we have done manually
- provision the steps of updating, upgrading and nginx installation
  
> vagrant up again
- redo all the steps 
- install nginx and load it in the browser 


vagrant up again
redo all the steps
install nginx and load it in the broswer

What is DevOps?
Fosters an environment of collaboration and trust as DevOps builds a culture of shared responsibility and faster feedback. Due to faster feedback loop, issues are resolved faster, and this minimises downtime. Faster release and work smarter as development and operations are not working in silos. Transparency leads to high productivity, and this also reduces the cost of production. This allows for more time to innovate rather than fix/maintain. Overall increasing customer satisfaction. 


""4 Principles of DevOps""

Continuous Flow
Ownership & Visibility (Outside-In)
Planning & Time Management
Culture

Engineering CI/CD Practices
Continuous Integration
Continuous Delivery 
Continuous Deployment

Challenges in New SDLC
- Ease of Use
- Flexibility
- Robustness
- Cost


""What is Piping""
In Linux, the pipe command lets you sends the output of one command to another. Piping, as the term suggests, can redirect the standard output, input, or error of one process to another for further processing.

Display first n lines from file cat file | head -n
Display last n lines from file cat file | tail -n
