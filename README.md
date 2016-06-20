# firm...s

*  In Linux http://linux.die.net/man/8/ebtables  does some of the tricks. 
*  Wireshark/pcap comes with a capture filter and language https://wiki.wireshark.org/CaptureFilters
*  http://www.cisco.com/c/en/us/products/collateral/security/ios-flexible-packet-matching-fpm/prod_qas0900aecd804b915e.html - can *not* handle non-IP protocols, CSCO FPM is almost there
*  MAC-based ACL
* Vadim says: probably big-ip


# Bottom line

On Linux : https://www.snort.org/ - regex, raw data, reconstruct the packets from fragments if needed.

NGREP - only Ehernet packets, very flexiblle pattern matching

Cisco has FPM - works only for IP traffic, but can be modified I imagine if they need it.

F5 Big-IP has a sniffer mode with regex pattern matching. Hard to configure and I am not sure how flexible it is. I have never worked with F5 equipment.
