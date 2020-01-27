## Accurate Per-Flow Packet Loss Monitoring in SRv6 

Segment Routing over IPv6 (SRv6) is a solution for IP backbones and Data Centers, which has been recently adopted in several large scale network deployments. A number of Internet Drafts have been submitted related to the Performance Monitoring of flows in an SRv6 network (SRv6-PM in short).

We present the implementation of a per-flow packet loss measurement (PF-PLM) solution based on the _alternate marking_ method. The implementation is based on Linux kernel networking and is open source. 

### Data plane based on iptables

Packet marking and counting based on iptables 

[srv6-pm-dp-iptables](https://github.com/netgroup/srv6-pm-dp-iptables)

(https://github.com/netgroup/srv6-pm-dp-iptables)

https://github.com/netgroup/srv6-pm-dp-iptables

### Data plane based on ipset

Packet marking and counting based on ipset extensions

https://github.com/netgroup/srv6-pm-dp-ipset

### Control plane 

Generation and processing of Loss Measurement Protocol Packets 

https://github.com/netgroup/srv6-pm-control
