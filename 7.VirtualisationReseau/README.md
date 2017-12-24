## Neutron 

Table of Contents
-----------------

  * [0.KVM](#0kvm) - Enabling `Kernel-Based Virtual Machine` Routing
  * [1.Bridging](#1bridging) - Routing with Bridges
  * [2.OpenVswitch](#2openvswitch) - Enabling Switching
  * [3.NetNS](#3netns) - Enabling User Network with Name Spaces
  * [4.p2p](#4p2p) - Connecting to the outside world a la P2P


### Quick overview

![alt tag](./NEUTRON.png)

### [0.KVM](./0.KVM)

* Modify the kernel to allow the routing of traffic between interfaces

![alt tag](./0.KVM/ROUTE.png)

### [1.Bridging](./1.Bridging)

* Setting up bridges critical to the operation of OpenStack networking

![alt tag](./1.Bridging/ISP.png)

### [2.OpenVswitch](./2.Open-vSwitch)

* What virtual switch is used in OpenSTack?

![alt tag](./2.Open-vSwitch/OVS.png)


### [3.NetNS](./3.NetNS)

* How to use NameSpaces to create separate tenant environments ?

![alt tag](./3.NetNS/namespace_level2.png)

### [4.p2p](./4.p2p)

* P2P (Peer to Peer - VM access) 

Connect the cloud to the external world

# References:

## Networking

hub vs Bridge vs Switch
https://www.youtube.com/watch?v=Xmwmezk75Tk

