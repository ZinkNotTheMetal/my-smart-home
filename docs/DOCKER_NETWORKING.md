# Network Chuck video w/ Timestamps

[Network Chuck - Docker Networking](https://www.youtube.com/watch?v=bKFMS5C4CG0)

Driver in Docker is equivalent to network type

[My current docker network setup](https://github.com/ZinkNotTheMetal/home-server-configuration/blob/main/roles/docker/tasks/create-network.yml)

## Default Bridge

[Default Bridge - NC YouTube](https://www.youtube.com/watch?v=bKFMS5C4CG0\&t=213s)

Cons:

* Manually expose ports for each service
* Could have multiple ports like 443 wanting to be used by multiple services

## User defined Bridge

[User-Defined Bridge - NC YouTube](https://www.youtube.com/watch?v=bKFMS5C4CG0\&t=644s)

```sh
docker network create <name>
```

Same as above just creating a bridge with a preferred name instead of **bridge**

Why?

* Network Isolation - you can separate containers into different networks that
don't need to be able to access each other

## Host

[Host Network - NC YouTube](https://youtu.be/bKFMS5C4CG0?t=942)

Pros:

* No ports needed to define
* Runs like an application on the host machine

Cons:

* No Isolation as it's next to the host

## MACVLAN

[Mac VLAN - NC YouTube](https://www.youtube.com/watch?v=bKFMS5C4CG0\&t=1050s)

Cons:

* Each docker container gets it's own MAC address (your network might not be able
to support multiple MAC address from one switch port)
* Port security
* Promiscuous mode (enable if you want to use this)
* No DHCP

Enable promiscuous mode in Linux

```sh
sudo ip link set <name of network controller> promisc on
```

## IPVLAN

[IPVLAN - NC YouTube](https://www.youtube.com/watch?v=bKFMS5C4CG0\&t=1501s)

This allows the host to share it's MAC address with the containers in the network.
This has the benefit of not having to worry about promiscuous mode and turning
that on, but they will have their own IP address

Two modes

* L2
* L3

Layer3 is very nice, but you will have to setup the network how to reach the subnet.
Also known as a static route.

Layer 3 setup

```sh
sudo docker network create -d ipvlan \
--subnet 192.168.xx.0/24 \
-o parent=<nic_name> \
-o ipvlan_mode=l3
--subnet 192.168.2.0/24 \
<name> 
```

Pros:

* Best practices

Cons:

* If you want separation between multiple ipvlanl3's you will need to connect
them to a different physical interface
* Static network needs to be setup on the network (Unifi can do this)

## Overlay network

[Overlay - NC YouTube](https://www.youtube.com/watch?v=bKFMS5C4CG0\&t=2200s)

If you have multiple hosts with multiple containers (Docker swarm)

## None network

Driver = null

## Useful commands

```sh
docker inspect <thing you want to inspect>
```
