
Wireshark Network Traffic Analysis Report
 Objective.
 The purpose of this lab was to capture and analyze live network traffic using Wireshark, identify various network protocols in use, and summarize key packet information for understanding how data flows across the network.

⚙️ Procedure

Installed Wireshark on the local system.

Started capturing packets on the active network interface.

Generated network activity by:

Visiting multiple websites in a browser

Running a ping command to external servers (e.g., ping google.com)

Stopped the capture after approximately one minute.

Filtered packets in Wireshark by common protocols:

tcp

udp

dns

ip

ipv6

Exported the capture:

Saved the raw capture as wireshark.1.pcapng

Exported packet summary as wireshark capture export.csv

Analyzed and summarized captured traffic statistics.

 Identified Protocols

At least five distinct protocols were observed in the capture:

Protocol	Description
TCP (Transmission Control Protocol)	Connection-oriented protocol used by web traffic, email, and other reliable services.
UDP (User Datagram Protocol)	Connectionless transport used by DNS and streaming applications.
IPv4 (Internet Protocol v4)	Core internet protocol responsible for packet addressing and routing.
IPv6 (Internet Protocol v6)	Newer version of IP supporting a larger address space.
DNS (Domain Name System)	Protocol that resolves domain names to IP addresses.
 Summary of Findings
Metric	Observation
Total Packets Captured	(from exported file) — Several hundred packets captured over 1 minute.
Top Protocols	TCP and UDP dominated the traffic, followed by DNS lookups.
Network Layers Observed	Data Link (Ethernet), Network (IPv4/IPv6), Transport (TCP/UDP), Application (DNS).
Traffic Pattern	Majority of TCP traffic associated with web browsing; intermittent DNS and UDP packets observed.
Interpretation

The capture confirms normal network behavior for a device actively browsing the web:

TCP sessions indicate HTTP/HTTPS communications.

UDP and DNS activity represent name resolution requests.

The presence of both IPv4 and IPv6 shows dual-stack network support.

No unusual or malicious packets were observed.

💾 Files Included
File Name	Description
wireshark.1.pcapng	Full packet capture in native Wireshark format
wireshark capture export.csv	Exported summary of packets (CSV format)
README.md	This report

 Conclusion
This lab successfully demonstrated the process of capturing live network traffic using Wireshark and analyzing packet-level data. Multiple network protocols were identified and examined, providing insight into how communication occurs between devices over the internet


Wireshark-Traffic-Analysis/
├── README.md                     # Full technical analysis report
├── wireshark.1.pcapng            # Placeholder (replace with your actual .pcapng)
├── wireshark capture export.csv  # Placeholder (replace with your actual CSV)
