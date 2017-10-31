# Demo Time!

1. sudo mn
2. h1 ifconfig
3. h1 <cmd> h2
    * ping
    * arp
    * traceroute

4. h2 python -m SimpleHTTPServer 80 >& /tmp/http.log &
5. h1 wget -O - h2
6. sudo mn --switch ovs --controller ref --topo tree,depth=2,fanout=8 --test pingall


* ping sweep -> for i in `seq 1 255`; do ping -c 1

* use *dump* and *links* data as input for [visualizer](http://mininet.spear.narmox.com/)
