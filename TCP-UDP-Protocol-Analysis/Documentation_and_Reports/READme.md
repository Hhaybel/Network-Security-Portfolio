# Analysis Documentation

This folder contains the results of my protocol investigation.

## 📄 Final Report
* **[Abel_Kolawole_Analysis_Report.pdf](./Abel_Kolawole_Analysis_Report.pdf)**: A full technical breakdown of TCP and UDP header fields and operational differences.

## 📸 Evidence Gallery
* `TCP_3way_Handshake.png`: Screenshot showing the SYN, SYN-ACK, ACK sequence.
* `UDP_Header_Analysis.png`: Visual evidence of the 8-byte UDP header.
* `Linux_Permissions_Fix.png`: Documentation of the `chown` fix used to manage file access in the VM.

## 🔍 Key Findings
Verified TCP header length of **40 bytes** (with options) for FTP and a fixed **8-byte** UDP header for TFTP, confirming the trade-off between reliability and overhead.

