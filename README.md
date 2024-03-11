# Simple Elastic SIEM Lab

## Objective

I’ll walk you through steps on how I set up a home lab for Elastic Stack Security Information and Event Management (SIEM) using the Elastic Web portal and a Kali Linux VM. I learned how to generate security events on the Kali VM, set up an agent to forward data to the SIEM, and query and analyze the logs in the SIEM.

### Skills Learned

- Set up and configured Elastic Stack SIEM in a home lab environment.
- Deployed a Kali Linux VM and configured Elastic Agents for log collection.
- Demonstrated proficiency in forwarding data to the SIEM for security event monitoring.
- Security Event Simulation and Analysis:

- Generated and analyzed security events using Nmap on Kali Linux.
- Acquired hands-on experience in querying Elastic SIEM to identify and investigate security incidents.
- Enhanced skills in network security monitoring and threat detection.
- Visualization and Alerting in SIEM:

- Developed a custom dashboard in Elastic SIEM for visualizing security events.
- Demonstrated skills in data interpretation and pattern recognition.
- Created and tested alert rules for detecting specific security events, showcasing competency in proactive incident response and alert management.

### Tools Used

- Elastic
- Kali Linux
- Oracle VM VirtualBox.

## Steps
1. Created an Elastic account
2. Downloaded Kali Linux on my host machiene and started a VM
3. I setup the agent to collect logs on Elastic
 
 ![image](https://github.com/hinksmon/Detection-Lab/assets/162920003/2f616d38-0cd6-4d6d-8e1f-8fbf4f44abf1)

4. Then I installed Elastic Defend and followed the instructions provided on the integration page to install the agent on your Kali VM.

![image](https://github.com/hinksmon/Detection-Lab/assets/162920003/9b284b40-50a0-4d62-9cf8-9d56a64f538f)

5. Once the agent is installed I saw a message that says “Elastic Agent has been successfully installed".

![image](https://github.com/hinksmon/Detection-Lab/assets/162920003/8eca03e3-2021-44f7-b58c-86e798179d28)

6After that I generated some traffic on my kali linux machiene with some basic nmap commands.

![image](https://github.com/hinksmon/Detection-Lab/assets/162920003/4a1e7357-29e4-479a-b27b-0029d094a815)

7. After generating the traffic I went to query for the security events in the Elastic SIEM

![image](https://github.com/hinksmon/Detection-Lab/assets/162920003/5e20733b-d82a-4e4a-a96e-99521ca3f3f6)

![image](https://github.com/hinksmon/Detection-Lab/assets/162920003/ce57bd4d-c41b-43ad-8788-a33f52480716)

8. Finally  I created an alert for my nmap commands that I ran on my VM, and had it saved so it can send to my email whenever i use nmap commands on my terminal.

![image](https://github.com/hinksmon/Detection-Lab/assets/162920003/afe2d1c3-e589-4cb2-ae77-181c685573dd)









