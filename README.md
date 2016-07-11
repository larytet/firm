# firm...s

*  In Linux http://linux.die.net/man/8/ebtables  does some of the tricks. 
*  Wireshark/pcap comes with a capture filter and language https://wiki.wireshark.org/CaptureFilters
*  http://www.cisco.com/c/en/us/products/collateral/security/ios-flexible-packet-matching-fpm/prod_qas0900aecd804b915e.html - can *not* handle non-IP protocols, CSCO FPM is almost there
*  MAC-based ACL
* Vadim says: probably big-ip


# Bottom line

On Linux : https://www.snort.org/ - regex, raw data, reconstruct the packets from fragments if needed (TCP fragments).

NGREP - only Ehernet packets, very flexiblle pattern matching

netsniff-ng includes Berkeley Packet Filter and Linux comes with BPF JIT compiler

Cisco has FPM - works only for IP traffic, but can be modified I imagine if they need it.

F5 Big-IP has a sniffer mode with regex (?) pattern matching. Hard to configure and I am not sure how flexible it is. I have never worked with F5 equipment.

Linux ebtables can be extended by custom code - kernel driver. 


# RegEx in FPGA

* http://halcyon.usc.edu/~pk/prasannawebsite/papers/sidhuFCCM01.pdf Fast Regular Expression Matching using FPGAs
* http://ac.els-cdn.com/S1877050914005134/1-s2.0-S1877050914005134-main.pdf?_tid=0f3cc23a-3892-11e6-97e3-00000aab0f02&acdnat=1466611245_985289a5f71b40d66b9e5e1d38e20b05#view=fit A Real-time Updatable FPGA-based Architecture for Fast Regular Expression Matching
* http://www.cs.ucr.edu/~najjar/papers/2007/ancs2007.pdf Compiling PCRE to FPGA for Accelerating SNORT IDS
* https://www.researchgate.net/publication/228810333_Efficient_FPGA_based_regular_expression_pattern_matching
* http://www.apsipa.org/proceedings_2011/pdf/apsipa268.pdf
* http://www.xilinx.com/programmable/about/research-labs/ANCS_final.pdf 400 Gb/s Programmable Packet Parsing on a Single FPGA 
* https://app.assembla.com/spaces/intelligentwires/documents/dVoEm0ojqr5RpcacwqjQXA/download/dVoEm0ojqr5RpcacwqjQXA  
* http://e-collection.library.ethz.ch/eserv/eth:297/eth-297-01.pdf
* 
