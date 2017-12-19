

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

