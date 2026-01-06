# Analysis Documentation

This folder contains the results of my protocol investigation.

## 📄 Final Report
* **[TCP-UDP-Protocol-Analysis/Documentation_and_Reports/TCP&UDP_Packet_Analysis_Report refined](./[TCP-UDP-Protocol-Analysis/Documentation_and_Reports/TCP&UDP_Packet_Analysis_Report refined.pdf)](https://github.com/Hhaybel/Network-Security-Portfolio/blob/main/TCP-UDP-Protocol-Analysis/Documentation_and_Reports/TCP%26UDP_Packet_Analysis_Report%20refined.pdf)**: A full technical breakdown of TCP and UDP header fields and operational differences.

## 📸 Evidence Gallery
*  (https://github.com/Hhaybel/Network-Security-Portfolio/blob/main/TCP-UDP-Protocol-Analysis/Documentation_and_Reports/Full%20TCP%20packet%20capture%20.png) Screenshot showing the SYN, SYN-ACK, ACK sequence.
* `UDP_Header_Analysis.png`: Visual evidence of the 8-byte UDP header.
* `Linux_Permissions_Fix.png`: Documentation of the `chown` fix used to manage file access in the VM.

## 🔍 Key Findings
Verified TCP header length of **40 bytes** (with options) for FTP and a fixed **8-byte** UDP header for TFTP, confirming the trade-off between reliability and overhead.

