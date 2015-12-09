# libpcap_openflow
openflow filtering patch for libpcap

* target : libpcap-1.7.4
* tcpdump command : ./tcpdump -i eth0 openflow [options]

# Current Support
* listening port
  * openflow port [port number]
  * default is 6633

# TODO
* Add option to filter openflow packets with specific types (e.g., packet_in, flow_mod, ...)
* Add option to filter openflow packets with specific values of fields (e.g., buffer_id == -1, ...)
