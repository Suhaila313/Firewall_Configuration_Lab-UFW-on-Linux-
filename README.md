Firewall Configuration Lab (UFW on Linux)
Task 4: Configure and test basic firewall rules using UFW.

📌 Overview
This lab demonstrates how to:

Block/allow traffic on specific ports (e.g., Telnet on 23, SSH on 22).

Test firewall rules and document the process.

Use UFW (Uncomplicated Firewall) on Linux.

🛠️ Tools Used
UFW (Uncomplicated Firewall)

Terminal commands

telnet (for testing)

🔧 Steps Reproduced
Check UFW Status:
sudo ufw status
Block Telnet (Port 23):

sudo ufw deny 23/tcp
Allow SSH (Port 22):

sudo ufw allow 22/tcp
Test Telnet Block:

telnet localhost 23
Delete Test Rules:

sudo ufw delete [rule-number]

📝 Key Learnings
✔ Firewalls filter traffic based on ports, IPs, and protocols.
✔ UFW simplifies rule management with allow/deny commands.
✔ Always test rules and document changes.

🔐 Security Note: Never expose sensitive ports (e.g., SSH) to public networks without additional safeguards like fail2ban.
