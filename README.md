# Course 4: System Administration and IT Infrastructure Services
## Student: Innocentia Jiwa
### Practical Task: Basic Apache Server Setup on Ubuntu (WSL)

---

### 📝 Project Overview
This project, completed by **Innocentia**, demonstrates the successful deployment of a local web server as part of the System Administration and IT Infrastructure Services curriculum. It covers the installation of server software, management of system services, and understanding of the Linux directory hierarchy within a virtualized environment.

---

### 🛠️ Configured Services & Infrastructure
* **Apache2 (Web Server):** A robust, cross-platform HTTP web server. I configured this service to listen on **Port 80** to handle incoming web traffic requests.
* **WSL (Windows Subsystem for Linux):** Used as a virtualization layer to run a Linux environment (Ubuntu 24.04) natively on a Windows 10/11 host.
* **Directory Services (Networking):**
   * **DHCP:** Utilized by the virtual network interface to automatically assign an IP address to the Linux instance.
   * **DNS/Loopback:** Leveraged the `localhost` address (127.0.0.1) to map the local hostname to the web server for testing.

---

### 📂 Folder Structure Explanation
A core competency of a System Administrator is managing the file system. The web content for this project is located at:
` /var/www/html/ `

* **The Document Root:** This is the standard directory where Apache looks for files to display to the public.
* **index.html:** The primary landing page file generated during the installation.
* **Permissions:** I utilized **Administrative Privileges** via the `sudo` command to ensure secure modification of these system-level files.

---

### 📸 Proof of Work (Screenshots)

#### 1. Service Status Confirmation
**![Server Status]
<img width="976" height="513" alt="apache running" src="https://github.com/user-attachments/assets/a5f18bfe-ec3e-48e3-92b3-9c6395a0faf2" />

* **Description:** This screenshot captures the output of the `sudo service apache2 status` command. It serves as proof that the Apache daemon is **active (running)**. Monitoring this state is a fundamental task for ensuring service availability.

#### 2. Linux Directory Hierarchy
**![Folder Structure]
<img width="978" height="515" alt="root" src="https://github.com/user-attachments/assets/563b16f6-f1f0-4435-9c09-66872c71a66c" />

* **Description:** This image shows the result of the `ls -l /var/www/html` command. It highlights the file permissions, ownership, and the presence of the `index.html` file within the system's web root.

#### 3. Successful Web Deployment (Browser View)
**![Webpage Confirmation]
<img width="1599" height="850" alt="screen apeche" src="https://github.com/user-attachments/assets/4c1122a0-a1a5-41e7-a69a-0391557c753b" />

* **Description:** The final verification step showing the "Apache2 Ubuntu Default Page" loaded in a Windows browser. This confirms that the server is correctly bridging the Linux subsystem to the local network.

---

### 🚀 Administrative Commands Executed
* `sudo apt update`: Refreshed the local package index to ensure the latest software versions.
* `sudo apt install apache2 -y`: Installed the web server infrastructure with an automated "yes" prompt.
* `sudo service apache2 start`: Manually initialized the web service.
* `ls -l /var/www/html`: Verified the directory structure and file existence.

---
*Developed by Innocentia as part of the IT Infrastructure Services Course.*
