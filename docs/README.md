## Accurate Per-Flow Packet Loss Monitoring in SRv6 

Segment Routing over IPv6 (SRv6) is a solution for IP backbones and Data Centers, which has been recently adopted in several large scale network deployments. A number of Internet Drafts have been submitted related to the Performance Monitoring of flows in an SRv6 network (SRv6-PM in short).

We present the implementation of a per-flow packet loss measurement (PF-PLM) solution based on the _alternate marking_ method. The implementation is based on Linux kernel networking and is open source. Please fine hereafter the source code repository of two data plane solution for packet marking and counting and one control plane solution for the generation and processing of Loss Measurement protocol packets.

### Data plane based on iptables

[srv6-pm-dp-iptables](https://github.com/netgroup/srv6-pm-dp-iptables) : Packet marking and counting based on iptables 


### Data plane based on ipset

[srv6-pm-dp-ipset](https://github.com/netgroup/srv6-pm-dp-ipset) : Packet marking and counting based on ipset extensions

### Control plane 

[srv6-pm-control](https://github.com/netgroup/srv6-pm-control) : Generation and processing of Loss Measurement Protocol Packets (based on scapy)
