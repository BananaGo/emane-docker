[![Build Status](https://travis-ci.com/gokarslan/emane-docker.svg?token=q3HaKjfJDzXzenoF3wmP&branch=master)](https://travis-ci.com/gokarslan/emane-docker)
[![Documentation Status](https://readthedocs.org/projects/emane-docker/badge/?version=latest)](https://emane-docker.readthedocs.io/en/latest/?badge=latest)

# EMANE-Docker

EMANE-Docker is a platform to deploy and emulate distributed wireless networks using [EMANE (Extendable Module Ad-hoc Network Emulator)](https://github.com/adjacentlink/emane) 


## Start using EMANE-Docker

1. Install Vagrant and VirtualBox on your machine.
2. Clone this repository by running git clone https://github.com/gokarslan/emane-docker.
3. Go to the emane-docker directory and run vagrant up. This command will bootstrap a VM running Ubuntu 16.04. Wait until Vagrant starts the VM and installs necessary packages.
4. SSH into the VM by running vagrant ssh.
EMANE-Docker requires sudo privileges. Run sudo su to switch to the root user.
6. Go to /root/emane-docker directory by running cd ~/emane-docker.
7. You can now run EMANE-Docker by simply running ./emane-docker --start. This will deploy the topology under emane_docker/topology.default.yaml. Please refer to Configuring EMANE-Docker for the details of configuring EMANE-Docker. This will start the EMANE-Docker CLI. You can run the following commands in the CLI:
- `start-experiment`: Starts the experiment.
- `start-event-generator`: Starts the event generator.
- `start-traffic-generator`: Starts the traffic generator.
- `help?`: Lists the available commands.
- `(stop || exit)`: Stops the topology.

8. You can destroy the VM by running vagrant destroy. This will stop and remove the VM. 

# Need more information?

Visit the EMANE wiki for more information about EMANE:

[https://github.com/adjacentlink/emane/wiki](https://github.com/adjacentlink/emane/wiki)

Visit EMANE-Docker documentation to get started:

[https://emane-docker.readthedocs.org](https://emane-docker.readthedocs.org)
