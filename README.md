# HW1
*DevOps Fall 17*


## Screencasts

**1.** [Running ansible play to setup mini-vlc](https://youtu.be/3uzOZu09ByU)

**2.** [phpVirtualBox demo](https://youtu.be/SIMAH2WMZA0)

**3.** [Installing vagrant and provisioning vm](https://youtu.be/5lfiNnrH6S8)


##  [Ansible Playbook](https://github.ncsu.edu/akshetty/HW1/blob/master/mini_vcl.yml)

## Approach

**1.** The basic idea was to convert each step in the guide to ansible tasks.

**2.** While most of the tasks were written using ansible modules, some of the tasks were required commands module.

**3.** I created two ubuntu/xenian nodes, one served as configuration server and the other as node server.

**4.** The phpVirtualBox only displays the preview of the hosted vm.

**5.** I assumed that the task was to automatically setup vagrant and provision a vm using ansible.
       The second idea coud've been to use ansible inside Vagrantfile and run ansible playbook, provisioning the server.
       This made little sense with the given HW description.

## Steps to create mini-vlc

**1.** 	Create an ubuntu/xenian 64 bit headless server using vagrant.
		
		*Useful Commands*:
		vagrant init ubuntu/xenian64
		vagrant up
		vagrant ssh

**2.**	Ensure that you can ping this server using ssh and ansible

**3.** 	An inventory file has been provided. You can change the ip as required.

**4.**	Run ansible playbook in mini_vlc.yml using command "ansible-playbook -i path/to/inventory path/to/mini_vcl.yml -s"

**5.**	Wait for installation.

**6.** 	Check if phpVirtualBox is up by running http:*node-ip*/phpvirtualbox/

**7.**	Check if vagrant vm is running in node server by running "vagrant ssh"
