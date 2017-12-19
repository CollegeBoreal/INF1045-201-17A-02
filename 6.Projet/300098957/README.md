

https://docs.openstack.org/devstack/latest/guides/single-machine.html

## Installation shake and bake

* Add your user

We need to add a user to install DevStack. 

```
$ sudo useradd -s /bin/bash -d /opt/stack -m stack
```

* Since this user will be making many changes to your system, it should have sudo privileges:

```
$ echo "stack ALL=(ALL) NOPASSWD: ALL" | sudo tee /etc/sudoers.d/stack
```

* Login as user stack

```
$ sudo su - stack
```

* Download DevStack

We’ll grab the latest version of DevStack via https:

```
$ sudo apt-get install git -y || sudo yum install -y git
$ git clone https://git.openstack.org/openstack-dev/devstack
$ cd devstack
```


* Edit the file local.conf

```
[[local|localrc]]
FLOATING_RANGE=10.13.237.48/28
FIXED_RANGE=172.16.0.0/24
FIXED_NETWORK_SIZE=256
FLAT_INTERFACE=enp10s0

ADMIN_PASSWORD=supersecret
DATABASE_PASSWORD=$ADMIN_PASSWORD
RABBIT_PASSWORD=$ADMIN_PASSWORD
SERVICE_PASSWORD=$ADMIN_PASSWORD
```

Run DevStack:

```
./stack.sh
```
