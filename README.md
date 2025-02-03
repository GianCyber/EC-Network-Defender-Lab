# EC-Network-Defender-Lab

## Objective

Understand and demonstrate the workings of various network attack and defense strategies, including XSS attacks, network scanning, and brute force attacks.


### Skills Learned

Advanced understanding of Cross-Site Scripting (XSS) attacks and payload injection techniques.
Practical application of network scanning tools and techniques to identify open ports and services.
Hands-on experience with brute force attack methods using Hydra and the importance of strong authentication mechanisms.
Improved knowledge of social engineering tactics and network security vulnerabilities.

### Tools Used


Hydra (Brute force tool)
Network scanning tools (e.g., Nmap)
Various network services for testing attacks (FTP, SMB, HTTP, etc.)

## Steps
Step 1: XSS Attack Demonstration

The exercise began by explaining how an attacker can exploit an XSS vulnerability in dynamically generated web pages. When content is not validated properly, an attacker can inject malicious scripts that get executed when a user visits the website.
The attacker, Bob, demonstrated this by logging into a website and sending a crafted email containing a script. The email included a social engineering element where the recipient was asked to "call" to "save data," a typical method used in these attacks.
This script, once executed, could lead to data theft if the recipient fell for the social engineering trick.

Step 2: Network Scanning

We then transitioned to network scanning, where the objective was to identify open ports on a target system.
Using Nmap, the attacker performed several types of scans: a TCP full connect scan, a UDP scan, and a scan for specific open ports. The Nmap command provided details of the ports open on the target system, including FTP, SMB, and HTTP services.
This helped identify potential points of vulnerability, such as open ports 21 (FTP), 80 (HTTP), 445 (SMB), and others.

Step 3: Brute Force Attack Using Hydra

The final part of the module covered brute force attacks. Hydra was used to attempt to crack the credentials for an FTP service.
Hydra works by testing hundreds or thousands of password combinations until it successfully authenticates. This is an example of a brute force attack where an attacker does not know the exact password but uses wordlists or known leaked credentials to attempt access.
The attacker showed how Hydra worked by running through possible combinations and successfully gaining access to the FTP service with the password “admin123.”
The demonstration also highlighted the importance of defenses against such attacks, including timeouts, account lockouts, and multi-factor authentication.

The final part of the module covered brute force attacks. Hydra was used to attempt to crack the credentials for an FTP service.
Hydra works by testing hundreds or thousands of password combinations until it successfully authenticates. This is an example of a brute force attack where an attacker does not know the exact password but uses wordlists or known leaked credentials to attempt access.
The attacker showed how Hydra worked by running through possible combinations and successfully gaining access to the FTP service with the password “admin123.”
The demonstration also highlighted the importance of defenses against such attacks, including timeouts, account lockouts, and multi-factor authentication.
