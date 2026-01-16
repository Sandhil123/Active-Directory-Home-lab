# Active-Directory-Home-lab
A home lab that mimics a real corporate office. I built a central Server to control security, used PowerShell code to instantly create **1,000 simulated employees**, and proved I could log in to a Windows 10 laptop using those new accounts.

## Network Architecture

<img width="1110" height="655" alt="image" src="https://github.com/user-attachments/assets/c5d5134a-04cc-483b-8813-132c275aab6e" />

## Successful Domain User Authentication from Client Machine
<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/f38c2d00-c397-4fee-abb3-0d60374872ce" />


## Tools & Technologies
- **Hypervisor:** Oracle VirtualBox 
- **Server OS:** Windows Server 2019 (Domain Controller) 
- **Client OS:** Windows 10 Enterprise 
- **Automation:** PowerShell ISE 


##  The Process
1.  **Server Configuration:** Deployed Windows Server 2019 and promoted it to a Domain Controller for `mydomain.com`.
2.  **User Management:** Created a dedicated Admin account to adhere to security best practice.
3.  **Networking Services:** Configured **NAT** to allow internal clients to access the internet and **DHCP** to automatically assign IP addresses.
4.  **Automation:** Wrote a PowerShell script to automatically generate over **1,000 user accounts** in seconds, simulating a bulk hiring scenario.
5.  **Client Testing:** Deployed a Windows 10 Enterprise client, joined it to the domain, and verified that the new users could log in.


##  Conclusion
This project successfully resulted in a fully functional Enterprise Active Directory environment.
- **Infrastructure:** A Domain Controller is now actively managing the network.
- **Connectivity:** Isolated client machines can access the internet securely via NAT.
- **Verification:** A Windows 10 Client successfully joined the domain, proving that centralized authentication work.

