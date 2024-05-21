# WirePlot
Introduction

WirePlot is a powerful, terminal-based tool that has been designed to promote the discipline of packet analysis and graphical data display in network architecture. This program provides network professionals, security experts, and curious enthusiasts with the capacity to generate, collect, and inspect network packets, allowing for a thorough understanding of network traffic patterns and protocol distributions.

WirePlot excels at simplifying difficult operations by offering a complete set of capabilities. Users may quickly create customized packets, integrate packet capture features with Wireshark, and do advanced packet analysis. This includes calculating latency, throughput metrics, and creating graphical representations to provide a comprehensive insight of network behavior and performance.


Objective

The primary objective of the WirePlot project is to develop a versatile, terminal-based tool for packet analysis and graphical representation. WirePlot aims to provide network professionals, security experts, and network enthusiasts with a comprehensive set of features and functionalities to:
Generate Customized Packets: Enable users to create network packets, specifying the destination IP, type of packets (TCP, UDP, HTTP, DNS, or random), and the number of packets to generate. This feature allows for tailored packet generation for various network analysis scenarios.
Capture Packets with Wireshark Integration: Seamlessly integrate with Wireshark, one of the most widely used packet capture tools, to initiate and control packet capture sessions directly from the WirePlot interface, enhancing ease of use and streamlining network monitoring.
Analyze Packet Data: Analyze captured packets from PCAP or PCAPNG files to gain insights into protocol distribution and network traffic patterns. WirePlot provides detailed breakdowns of packet types and protocol usage.
Calculate and Visualize Data: Calculates the required parameters and generate a variety of graphical representations, including bar graphs, pie charts, and so on, to make network data more comprehensible and actionable.

Network Parameters Monitored 

    1. Latency 
    2. Throughput
    3. Time to Live
    4. Jitter
    5. Bandwidth

Packet Attributes

    1. Source IP – 172.20.17.23, Subnet: 255.255.248.0, Group B
    2. Destination IP – 8.8.8.8, Subnet: 255.255.255.0, Group A
    3. Source Port – 64657
    4. Destination Port  - 53
    5. Protocol – TCP, UDP, HTTP, DNS, ICMP 
    6. Packet Size –1500 bytes
    7. Packet Count – 14199
    8. Flags set in the packet – S (Stream flag)

There are 3 steps I did to create the whole experiment

1st Step

I made a simple python script using python using the scapy module to analyze a pcap
file and find the throughput, latency and other factors of the packets and a graph that shows the
Number of packets vs Protocols graph.

2nd Step

Expanded the capabilities of our program as follows:

• Created a terminal menu-based program.

• Opens Wireshark from terminal for packet analysis.

• Reads pcap file, measures and displays the necessary network parameters as output.

• Graph for each network parameter for each packet can be visualized individually.

• Added multiple types of graphical representation like bar graph, Pie graph and so on.

3rd Step

I upgraded the code in Step 2 and added more capabilities to our program as follows:

• Opens Wireshark from terminal for packet analysis and the program now waits until you
close Wireshark.

• The pcap/pcapng file can be read and the network parameters mentioned are calculated
and displayed accordingly along with their graph (which can be disabled if needed).

• Added functionality to send packets, now the user can send random packets (multiple
protocols) or send multiple packets of any user-specified protocol.

• Graphical representation has been improved and few bugs found were fixed.

Conclusion

In the world of networking, understanding what's happening with your data is crucial. That's
where WirePlot comes in. WirePlot is a user-friendly, terminal-based tool that makes the
complex task of packet analysis a breeze. It lets you generate custom packets, capture packets
using Wireshark, and dive deep into your data by analyzing PCAP or PCAPNG files.
With WirePlot, you can explore network performance with ease. It calculates latency,
throughput, and other network parameters and it even shows you the types of packets flowing
through your network. Plus, it visualizes all this data with various graphing options like bar
graphs, line graphs and so on.

This project aims to make networking more accessible and insightful. As networks continue to
evolve, tools like WirePlot will be essential in ensuring our networks operate efficiently and
securely. So, whether you're a seasoned pro or just getting started, WirePlot has your back in
the world of networking.
