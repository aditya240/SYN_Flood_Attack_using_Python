# SYN_Flood_Attack_using_Python

Overview

This Python script demonstrates how to perform a SYN Flood attack using the Scapy library. A SYN Flood attack is a type of Denial of Service (DoS) attack where an attacker sends a succession of SYN requests to a target's system in an attempt to consume enough server resources to make the system unresponsive to legitimate traffic.

Requirements

Python 3.x
Scapy library: Can be installed using pip install scapy
How to Use

Run the script from the command line, providing the target IP address and port number as arguments.

python3 synflood.py <Target-IP> <Port-Number>

For example:

python3 synflood.py 192.168.1.1 80

How it Works

The script checks if the required command line arguments (IP address and port number) are provided. If not, it prints the usage information and exits.
The IP and TCP layers of the packet are defined using Scapy. The destination IP address and port number are set according to the user's input. The TCP layer is set with the SYN flag to initiate a TCP connection.
An infinite loop is started to continuously send packets.
For each packet, random values are generated for the source IP address, source port number, and TCP sequence number to make each packet unique and harder to filter out.
The packet is sent to the target IP address and port number.
Security Implications

This script is a demonstration of a SYN Flood attack, which is illegal and unethical to perform on any network or system without explicit permission.
The purpose of this script is educational, to help understand how SYN Flood attacks work and how they can be mitigated.
Running this script against any unauthorized network or system can lead to severe consequences, including legal actions.
Disclaimer

This script is provided for educational purposes only. Using this script for attacking targets without prior mutual consent is illegal. It is the end user's responsibility to obey all applicable local, state, and federal laws. The author assumes no liability and is not responsible for any misuse or damage caused by this program.
