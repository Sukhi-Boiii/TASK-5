Cyber Security Internship - Task 5: Packet Capture and Analysis using Wireshark

objective: >
  Capture live network traffic using Wireshark, identify common protocols, 
  and understand how packet-level communication works. The aim was to get familiar 
  with packet structure and protocol filtering.

tools_used:
  - Wireshark (GUI packet analyzer)
  - Internet Browser (to generate traffic)
  - Terminal (used to ping domains)

steps_performed:
  - step: Installed Wireshark
    command: sudo apt install wireshark

  - step: Launched Wireshark and selected the active network interface (wlan0)

  - step: Started live capture

  - step: Opened browser and visited:
    sites:
      - google.com

  - step: Ran ping command in terminal
    command: ping google.com

  - step: Let Wireshark capture for ~1 minute, then stopped capture

  - step: Applied filters to analyze specific protocols
    filters:
      - dns
      - http
      - tcp

  - step: Identified 3 protocols:
    protocols:
      - DNS
      - HTTP
      - TCP

  - step: Exported the capture as capture-task5.pcap

files_in_repo:
  - task5.pcap
  - questions.md

what_i_learned:
  - A packet is a unit of data transferred over a network.
  - Wireshark captures and displays real-time traffic on network interfaces.
  - Protocol filters like dns, http, tcp help narrow analysis.
  - TCP is connection-based; UDP is faster but connectionless.
  - DNS queries resolve domain names into IP addresses.
  - Packet capture is useful for diagnosing network issues.

summary: >
  Wireshark is a powerful tool for analyzing network activity. This task helped 
  me understand how data moves over a network, how to apply protocol filters, 
  and how to export and review captured traffic for learning and troubleshooting.

outcome: >
  Hands-on experience with network traffic capture and protocol-level 
  observation. Developed basic skills in filtering, identifying and interpreting packets.
