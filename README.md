<h1>Business Email Compromise Investigation</h1>

Overview

This project involved investigating a simulated Business Email Compromise (BEC) attack by analyzing PCAP files in Wireshark.

Tools Used:
Wireshark,
PCAP Analysis,
SMTP / IMF,
Network Forensics,
TCP/IP

## INVESTIGATION

I analyzed multiple .pcap files in Wireshark and used smtp and imf filters to isolate and examine email traffic.

<img width="1920" height="992" alt="cybersecurity project1 (wireshark)" src="https://github.com/user-attachments/assets/f9ca8440-946a-485a-b137-834bc6644115" />

Through my analysis, I identified 24 phishing emails. I examined their subject lines, message data, and associated network traffic to trace the malicious activity back to its source.

<img width="1920" height="1013" alt="wireshark filter imf 2" src="https://github.com/user-attachments/assets/f133063b-40f6-45a4-8ad4-37eb138148a4" />

## Key Findings

- **24** phishing emails identified
- Malicious Source IP: 10.6.1.104
- Correlated suspicious email activity with SMTP/IMF network traffic
- Used email metadata and packet information to distinguish malicious
messages from legitimate traffic

## Network Analysis

The malicious SMTP traffic observed in the packet capture originated from
`10.6.1.104`.

Because `10.6.1.104` is a private IPv4 address, I learned that an IP address
observed in a packet capture must be interpreted based on where the traffic
was captured. A packet captured before NAT can show a private source IP,
while traffic observed after NAT may show a translated public IP address.

This reinforced the importance of using network metadata and capture context
when analyzing suspicious activity.

## Skills Practiced

Wireshark
Network Traffic Analysis
PCAP Analysis
SMTP/IMF Analysis
Phishing Investigation
Network Forensics
Key Takeaway

## Conclusion

This project strengthened my ability to analyze packet captures, identify phishing activity, and use network metadata to trace suspicious communications back to their source.

