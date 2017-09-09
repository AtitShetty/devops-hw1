# HW1
*DevOps Fall 17*


## Screencasts

**1.** [Running ansible play to setup mini-vlc]()

**2.** [phpVirtualBox demo](https://youtu.be/SIMAH2WMZA0)

**3.** [Installing vagrant and provisioning vm](https://youtu.be/5lfiNnrH6S8)


##  [Ansible Playbook]()

## Approach

**1.** The basic idea was to convert each step in the guide to ansible tasks.

**2.** While most of the tasks were written using ansible modules, some of the tasks were required commands module.

**3.** I created two ubuntu/xenian nodes, one served as configuration server and the other as node server.

**4.** The phpVirtualBox only displayed the preview of the hosted vm.

**5.** I assumed that the task was to automatically setup vagrant and provision a vm using ansible.
       The second idea coud've been to use ansible inside Vagrantfile and run ansible playbook, provisioning the server.
       This made little sense with the given HW description.
