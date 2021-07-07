### Notes

#### Vagrant

I started by using Vagrant to create virtual machines on my local machine and provision using Ansible from within the Vagrant script.

However after getting this working I wanted to create a virtual machine within DigitalOcean and this proved to be non-trivial.  So I decided this wasn't worth the investment in time as the bulk of the effort had been into getting the Ansible playbook working.

So I created the DigitalOcean Droplets "by hand" using the DO website, but then used the same Ansible playbook to provision them.

This worked very well.

So while the Vagrant infrastructure that I created is still here, I am not using Vagrant at all in my production Devops.

#### The Future

I may well still use Vagrant to create a local test environment for the app but at the moment the workflow of coding and testing from within the IDE (PyCharm) and then deploying to the BlueGreen environment and switching once working seems to be a good one and I may not need anything more complex.