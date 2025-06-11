# aws-secure-web-server
## Project Goal
To deploy a public-facing web server on AWS while implementing strong network security controls to protect it from unauthorized access.

## Solution Overview
This project involved setting up a robust and isolated cloud network (VPC) to host a simple web server (Nginx on EC2). The core security mechanism was the configuration of AWS Security Groups, acting as a stateful firewall, to precisely control incoming and outgoing network traffic. This demonstrates the principle of least privilege by allowing only necessary access.

---

## AWS Services Used
* **Amazon VPC (Virtual Private Cloud):** Created an isolated, private network.
* **Amazon EC2 (Elastic Compute Cloud):** Hosted the virtual web server instance.
* **Security Groups:** Acted as virtual firewalls to control instance-level traffic.
* **Internet Gateway (IGW):** Enabled communication between the VPC and the internet.
* **Route Tables:** Defined network traffic paths within the VPC and to the internet.

---

## Key Security Concepts Demonstrated
* **Network Segmentation:** Implemented through the use of VPCs and subnets to logically separate network resources.
* **Virtual Firewalls:** Configured Security Groups to filter traffic based on port and source/destination IP.
* **Principle of Least Privilege:** Applied by restricting SSH access to only specific IP addresses.
* **Cloud Deployment & Infrastructure as Code (Conceptual):** Demonstrated the ability to provision and configure cloud resources.

---

## Verification
The web server was successfully accessed via HTTP, demonstrating that the Security Group rules allowed legitimate web traffic. SSH access was also verified from my specific IP, confirming restricted administrative access.

---

## Screenshots

### Web Server Output
*(Replace with your screenshot)*
![Web Server Output](https://github.com/YosifYolen/aws-secure-web-server/blob/main/Hello%20from%20my%20secure%20web%20server%20on%20AWS!.JPG?raw=true)

### Security Group Inbound & Outbound Rules
*(Replace with your screenshot)*
![Security Group Inbound & Outbound Rules](https://github.com/YosifYolen/aws-secure-web-server/blob/main/Inbound%20&%20Outbound%20Rules.JPG?raw=true)

---

## Lessons Learned
* Gained hands-on experience with fundamental AWS networking services (VPC, Subnets, IGW, Route Tables).
* Solidified understanding of how Security Groups function as instance-level firewalls and their importance in cloud security.
* Emphasized the critical nature of configuring inbound and outbound rules meticulously to ensure security while maintaining necessary accessibility.
* Understood the necessity of proper resource cleanup in cloud environments to manage costs and security posture.
