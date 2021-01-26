## Accurate Per-Flow Packet Loss Monitoring in SRv6 

Segment Routing over IPv6 (SRv6) is a solution for IP backbones and Data Centers, which has been recently adopted in several large scale network deployments. A number of Internet Drafts have been submitted related to the Performance Monitoring of flows in an SRv6 network (SRv6-PM in short).

We present the implementation of a per-flow packet loss measurement (PF-PLM) solution based on the _alternate marking_ method. The implementation is based on Linux kernel networking and is open source. Please fine hereafter the source code repository of two data plane solutions for packet marking and counting and one control plane solution for the generation and processing of Loss Measurement protocol packets.

This project is part of the [ROSE project](https://netgroup.github.io/rose/).

### Data plane based on iptables

[srv6-pm-dp-iptables](https://github.com/netgroup/srv6-pm-dp-iptables) : Packet marking and counting based on iptables 


### Data plane based on ipset

[srv6-pm-dp-ipset](https://github.com/netgroup/srv6-pm-dp-ipset) : Packet marking and counting based on ipset extensions

### Control plane 

[rose-srv6-control-plane](https://github.com/netgroup/rose-srv6-control-plane) : Generation and processing of Loss Measurement Protocol Packets (based on scapy)

### Data plane 
[rose-srv6-data-plane](https://github.com/netgroup/rose-srv6-data-plane)

### The Mininet topology 
The Mininet topology used in the loss monitoring experiments is called 8r-1c-srv6-pm and it can be found in this repo:
[rose-srv6-tutorial](https://github.com/netgroup/rose-srv6-tutorial)



### Scientific papers 

- P. Loreti, A. Mayer, P. Lungaroni, F. Lombardo, C. Scarpitta, G. Sidoretti, L. Bracciale, M. Ferrari, S. Salsano, A. Abdelsalam, R. Gandhi, C. Filsfils,<br>
["SRv6-PM: A Cloud-Native Architecture for Performance Monitoring of SRv6 Networks"](https://arxiv.org/pdf/2007.08633.pdf),<br>
accepted for publication in IEEE Transaction on Network and Service Management, special issue on “Advanced Management of Softwarized Networks” ([pdf-preprint](https://arxiv.org/pdf/2007.08633.pdf))

- P. Loreti, A. Mayer, P. Lungaroni, S. Salsano, R. Gandhi, C. Filsfils,
"[Implementation of Accurate Per-Flow Packet Loss Monitoring in Segment Routing over IPv6 Networks](https://arxiv.org/pdf/2004.11414)", 
IEEE International Conference on High Performance Switching and Routing, (HPSR 2020), 11-14 May 2020, Virtual Conference. 
