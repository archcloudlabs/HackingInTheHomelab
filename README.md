# HackingInTheHomelab
Resources for all things related to hacking in the homelab.
Related personal projects can be seen [here](https://wwww.archcloudlabs.com/projects).

## Homelab Virtualization & Infrastrucre Management Resources
### Infrastructure - Local
Looking to deploy some VMs? Wondering what to use? Consider your usecase around
the hardware you have and if you want to spend money or not.  Maybe you can get
away with deploying some containers (ex: if you're just deploying Kali for
the metasploit framework ). If chosing VMWare ESXi, be sure to check if your hardware can support ESXi. Note that some
"unsupported" devices still do run but there's no guarantee it'll be supported
in the long run. A great example of this is the [Intel NUC](https://www.virtuallyghetto.com/2020/01/esxi-on-10th-gen-intel-nuc-frost-canyon.html).

* [VMUG - PAID, but lots of VMWare products cheap](https://www.vmug.com/home)
* [KVM](https://help.ubuntu.com/community/KVM/Installation)
    * [Virtmanager](https://virt-manager.org/)
    * KVM + Virtmanager is my 2nd choice if ESXi is out of the question.

* [Docker](https://docs.docker.com)
    * In my experience things get weird with Docker on OS X/Windows. Particualrly from a networking perspective.
    If you're deploying containers, a Linux host/VM is going to result in the
    best experience.

* [Virtualbox](https://www.virtualbox.org/)
    * Great to use w/ [Vagrant](https://www.vagrantup.com/)
    * Networking options are different than other offerings and in my opinion
      less intutitive to use.

#### Agentless Deployments
* Automate your deployments w/ [Ansible](https://docs.ansible.com/)
    * All you need is SSH and you can deploy and configure your machines.
    * Looking for example playbooks? Checkout [ansible-galaxy](galaxy.ansible.com).
    * Looking for a project to contribute to? Checkout [kali-up](https://www.github.com/archcloudlabs/kali-up).

#### Agent Based Deployments
* Automate your deployments w/ [Chef](https://docs.chef.io/)
* Automate your deployments w/ [Salt](https://docs.saltproject.io/en/latest/)
