# libpcap\_openflow
openflow filtering patch for libpcap

* target : libpcap-1.7.4
* tcpdump command : ./tcpdump -i eth0 openflow [options]

# Current Support
* listening port
  * openflow port [port number]
  * default is 6633
* filter openflow type
  * openflow oftype [type name]
  * list of type names
    * OFPT\_HELLO : "hello"
    * OFPT\_ERROR : "error"
    * OFPT\_ECHO\_REQUEST : "echo\_request"
    * OFPT\_ECHO\_REPLY : "echo\_reply"
    * OFPT\_VENDOR : "vendor"
    * OFPT\_FEATURES\_REQUEST : "features\_request"
    * OFPT\_FEATURES\_REPLY : "features\_reply"
    * OFPT\_GET\_CONFIG\_REQUEST : "config\_request"
    * OFPT\_GET\_CONFIG\_REPLY : "config\_reply"
    * OFPT\_SET\_CONFIG : "set\_config"
    * OFPT\_PACKET\_IN : "packet\_in"
    * OFPT\_FLOW\_REMOVED : "flow\_removed"
    * OFPT\_PORT\_STATUS : "port\_status"
    * OFPT\_PACKET\_OUT : "packet\_out"
    * OFPT\_FLOW\_MOD : "flow\_mod"
    * OFPT\_PORT\_MOD : "port\_mod"
    * OFPT\_STATS\_REQUEST : "stats\_request"
    * OFPT\_STATS\_REPLY : "stats\_reply"
    * OFPT\_BARRIER\_REQUEST : "barrier\_request"
    * OFPT\_BARRIER\_REPLY : "barrier\_reply"
    * OFPT\_QUEUE\_GET\_CONFIG\_REQUEST : "queue\_config\_request"
    * OFPT\_QUEUE\_GET\_CONFIG\_REPLY : "queue\_config\_reply"
  * simple arithmetic
    * openflow oftype [type name] or [type name]

# TODO
* Support arithmetics
* Add option to filter openflow packets with specific values of fields (e.g., buffer\_id == -1, ...)
