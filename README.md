Objective
This project demonstrates the process of scanning a local network for open ports to
understand network service exposure,as per the internship task.


Tools Used
Nmap: A powerfull network discovery and security auditing tool.
Ubuntu: The operating system used to perform the scan.


Process
1.initial scan: I performed a full TCP connect scan (-sT) to identify active hosts and
                their open ports on the network range 192.168.155.0/24

2.Saving results: The scan output was saved to a text file for documentation using the -oN
                  full_scan_results.txt


Findings
The scan successfully identified two active hosts with open ports
     .host1: 192.168.155.21
          .port 22/tcp: This port is open and is associated with the SSH service.
                        This indicates that this device can be remotely accessed and managed securely

     .host2: 192.168.155.224 (my own machine)
          .port 80/tcp: This port is open and is associated with HTTP service.
                        This indicates that the web server is running on this device.

The detailed results and output from the terminal are attached in the full_scan_results.txt file
and also shown in the screenshots below.



