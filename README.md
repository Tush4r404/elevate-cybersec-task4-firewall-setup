# Elevate Cybersecurity Internship - Task 4: Firewall Setup on Windows

## Objective:
Configured and tested firewall rules on Windows using Windows Defender Firewall to block and allow specific traffic.

## Tools Used:
- Windows Defender Firewall
- Windows CMD for testing
- Telnet Client

## Steps Performed:
1. Opened Windows Defender Firewall with Advanced Security.
2. Created a new inbound rule:
   - Type: Port
   - Protocol: TCP
   - Port: 23
   - Action: Block the connection
   - Profile: All
   - Name: Block Telnet Port 23
3. Enabled the Telnet Client:
   dism /online /Enable-Feature /FeatureName:TelnetClient
4. Tested the rule using:
   telnet localhost 23
   The connection failed, confirming that port 23 was blocked.
5. Removed the block rule from Windows Defender Firewall.

## Screenshots:
- Rule creation
- Telnet connection failure
- Rule removal

## Firewall Traffic Filtering Summary:
A firewall filters network traffic based on defined rules. It decides whether to allow or block traffic based on ports, protocols, or application rules. In this task, port 23 was blocked to prevent insecure Telnet connections.

## Repository Contents:
- screenshots folder
- README.md
- Interview_Questions.md

## Conclusion:
Successfully demonstrated basic firewall management on Windows by blocking port 23, testing the block, and restoring the system to its original state.
