# Sam Orlov 
www.linkedin.com/in/sam-orlov
# Summary
Sam has a diverse background in the Information Technologies field, with experience spanning IT infrastructure maintenance to designing communication systems. He specializes in DevOps and network engineering, including CI/CD pipelines (Jenkins, GitLab CI/CD, GitHub Actions), Infrastructure as Code (Terraform, Ansible), and containerized environments (Docker Compose, Kubernetes). He builds and maintains monitoring and logging systems (Prometheus, Grafana, ELK, Zabbix) and manages AWS services (EC2, Lambda, S3).

His experience includes commissioning and supporting drone-in-a-box sites, creating a Prometheus/Grafana monitoring platform, automating network fleets with Ansible, configuring PLCs, and working on large ISP and OT/IT deployments (Power of Siberia). He is proficient in Python, Groovy/Java, SQL, C#, Bash, HCL, and JavaScript, demonstrated through TAFE projects such as the WareLog Android App (.NET MAUI), WareLog-API (FastAPI), and a mobile-first web project with Tailwind CSS.

Sam is currently studying a Diploma in Advanced Programming and holds CKA and AWS Solutions Architect – Associate certifications
# Skills
- **DevOps**: CI\\CD, Jenkins, Ansible, Docker Compose, Terraform, Artifactory, GitOps, GitHub Actions, GitLab CI/CD, Vault  
	- **Orchestration & Virtualisation**: Kubernetes, Proxmox
	- **Monitoring & Logging**: Prometheus, Grafana, ELK, Zabbix, Telegraf, MQTT
	- **Version Control**: Git (Bitbucket, GitLab, GitHub)
- **Amazon Web Services**: EC2, Lambda, S3, Step Functions, DMS, CloudFormation
- **Program languages**: Groovy, Python, SQL, C# (.NET MAUI), JavaScript (Tailwind CSS), bash, HCL (Terraform), PromQL (Prometheus)
- **Network Administration**: Routing, TCP/IP, OSPF, VRRP, RSTP, VPN, WireGuard DNS, DHCP, SD-WAN, QinQ ([802.1ad](https://www.google.com/search?q=802.1ad&ved=2ahUKEwiCocOvq56SAxVDPhAIHSX9FoMQgK4QegYIAQgAEAU)), LLDP, tcpdump

# Projects
- [*MetricMonkeys* Monitoring Platform (Prometheus & Grafana)](#metricmonkeys-monitoring-platform-prometheus--grafana)
- [Pull Request Merge Readiness Validation](#pull-request-merge-readiness-validation)
- [Power of Siberia Gas Pipeline - OT & IT Network Deployment](#power-of-siberia-gas-pipeline--ot--it-network-deployment)
- [Deployed and integrated Artifactory](#deployed-and-integrated-artifactory)
- [Designed and implemented an Ansible](#designed-and-implemented-an-ansible)
- [ISP Network Deployment](#isp-network-deployment)
- [Dalet System Deployment (News Production & Distribution system)](#dalet-system-deployment-news-production--distribution-system)
- [WareLog Android App (.NET MAUI)](#warelog-android-app-net-maui)
- [WareLog-API (fastAPI)](#warelog-api-fastapi)
- [Web project (Tailwind CSS)](#web-project-tailwind-css)
  
# Career history
## **Automation Engineer** at RocketDNA (WA) Pty Ltd
Jun 2025 - Present
[RocketDNA](https://www.rocketdna.com/) is a global technology company that leverages AI and autonomous drones to provide geospatial data, automation and aerial surveying solutions for enterprise customers in mining, agriculture and critical industries.  
### Responsibilities
- Commissioning of new **drone-in-a-box** (DJI Drone & DJI [Dock](https://enterprise.dji.com/dock-3)) systems across multiple sites:
	- Configure **Teltonika network devices**(RUTX series), using **4G/5G** as a secondary connectivity link for the dock systems
	- Set up **Starlink uplinks** or coordinate integration with **site-provided networks**, including **port forwarding** on corporate network infrastructure
	- Configure **PLCs (Allen-Bradley Micro820)** using **Connected Components Workbench (CCW)** to control and monitor **low-voltage systems**
	- Deploy and integrate **Victron Energy solar inverter and battery systems** when required
	- Configure operational support systems, including **CCTV cameras** and **weather stations**
	- **Configure radio gateway systems** (based on **iCom VE-PG4**) to enable remote pilots in the **Remote Operations Center** to stream radio broadcasts from flight locations.
	- Organise **logistics and purchasing** using **Cin7**, ensuring timely delivery of equipment and spare parts
- Maintenance of **drone-in-a-box** systems on sites (11 installations):
	- Monitor on-site infrastructure, including **DJI Docks**, **Teltonika routers**, **Starlink dishes**, and **solar inverter and battery systems**
	- Perform drone servicing and maintenance, including **complex maintenance on site** and **simple maintenance coordinated with local site teams**
	- Conduct **test flights after servicing** to verify operational readiness
	- Oversee **drone battery management**, including charging cycles, health monitoring, and replacement planning
	- Troubleshoot and resolve **hardware, connectivity, and operational issues** related to drones and dock systems
	- Manage **logistics and stock receiving** for drone equipment and spare parts
	- Maintain accurate **inventory records** across all sites	
- Automate internal operational and data-handling processes using **scripting and Microsoft Power Automate**, reducing manual workload and improving system reliability.

### Project
#### *MetricMonkeys* Monitoring Platform (Prometheus & Grafana)
https://github.com/Dezkiy/MetricMonkeys
Architect, deploy and maintain data collection and monitoring infrastructure (**Prometheus** & **Grafana**) for **drone-in-a-box** systems operating on active mining sites:
- Organize, collect, process, and store device, operational, and business metrics from multiple data sources including DJI FlightHub2 metrics and network equipment.
- Transform raw, unstructured telemetry (**MQTT**) and **SNMP** data into structured Prometheus metrics suitable for analysis and visualization
- Design and configure **Alertmanager** rules to detect critical conditions and send automated notifications to **Microsoft Teams**
- Design, develop, and maintain **Grafana dashboards** for real-time monitoring and analysis of device, network, and business metrics
- **Build and manage the monitoring platform using Infrastructure as Code**, deployed on **Proxmox**, and fully containerized with **Docker Compose**
##### Planned features:
- **Modbus** to MQTT integration for low-voltage monitoring
- **gRPC**-to-Prometheus metric transformation for Starlink dish telemetry
- Multi-source weather data aggregation (BOM, Windy) visualized in Grafana
- **Victron Energy solar inverter and battery system integration**, monitoring inverter performance, battery state of charge, power flow, and system health metric

## **DevOps Engineer** at 2GIS
May 2021 - Sep 2023 (2 years 5 months)  
[2GIS](https://dev.2gis.ru/en/company) is an international geospatial company that develops detailed digital city maps, navigation services, and local business search platforms.
### Responsibilities
- Support and develop the main Continuous Integration (CI) pipeline based on **Jenkins**:
	- Develop and maintain **shared libraries (Groovy)** to improve efficiency and standardize CI processes across projects
	- Work with **HashiCorp Vault** in CI processes to securely consume secrets (credentials, tokens, API keys) used by Jenkins pipelines
	- Analyse metrics and logs from different pipeline stages using **ELK Stack** and **Prometheus**, identifying bottlenecks and optimizing performance
	- Administer and maintain build nodes (**Windows, Ubuntu, macOS**) using **Ansible**
	- Design and implement **alerts and notifications** in **Slack** to ensure timely incident response and pipeline monitoring
	- Optimize Jenkins by removing legacy plugins, simplifying maintenance, and improving overall server performance
- Maintain and support secondary CI pipelines based on **GitLab CI/CD**
- Collaborate with development teams to establish and maintain a new testing pipeline, streamlining the transition from the legacy system, improving testing speed, and optimizing hardware utilization
- Ensure CI and testing environments are properly configured, maintained, and aligned with development and release requirements
- Provide support to developers on CI/CD-related issues, ensuring smooth pipeline operations and rapid resolution of build or deployment problems
### Projects
- #### Pull Request Merge Readiness Validation
  **Designed and developed an internal shared library (Java/Groovy)** for merge validation, checking the feasibility of merging pull requests by querying **GitLab and Bitbucket APIs** for branches and active pull requests, with automated notifications sent to **Slack** and **Jira** in the context of related tickets.
- #### Deployed and integrated Artifactory
  Deployed and integrated Artifactory into the CI ecosystem, standardising artifact storage and delivery
## **Network Engineer** at LLC Gazprom transgaz Tomsk
Apr 2017 - May 2021 (4 years 2 months)
[**LLC Gazprom transgaz Tomsk**](https://institute.gazprom.ru/en/) operates and maintains extensive gas transportation systems across Siberia and the Russian Far East, ensuring reliable delivery of natural gas through thousands of kilometres of main pipelines.
### Responsibilities
- Deploy, configure, and administer enterprise network equipment from vendors including **Cisco, Huawei, Eltex**, and **HP**
- Design and maintain **OSPF**-based routed network architecture to ensure scalable and efficient traffic flow
- Implement network redundancy and high availability solutions, including **VRRP**, following industry best practices
- Monitor network performance and availability using **Zabbix**, ensuring high reliability and rapid incident response
- Troubleshoot network issues using **tcpdump** and **Wireshark** to analyze traffic and identify root causes
- Coordinate with cross-functional teams for smooth deployment of IT/OT systems
- Apply network security, troubleshooting, and automation best practices to maintain large-scale corporate network infrastructure
- Provide technical support to users and clients, ensuring minimal downtime and optimal service quality
### Projects
- #### Power of Siberia Gas Pipeline – OT & IT Network Deployment
    Participated in the construction and deployment of OT and IT networks along the **[Power of Siberia](https://en.wikipedia.org/wiki/Power_of_Siberia)** gas pipeline:
  - Designed and deployed networks for two sites, including a compressor station and a operations facility, ensuring reliable and secure connectivity.
  - Configured and installed network equipment in remote sections of the gas pipeline.
- #### Designed and implemented an Ansible 
  Designed and implemented an Ansible-based network automation system to centrally administer and orchestrate network devices, significantly improving troubleshooting speed, configuration consistency, and operational efficiency
## **Design Engineer** at Elcomplus LLC
Feb 2014 - Apr 2017 (3 years 3 months)
[Elcomplus](https://www.smartptt.com/) is an international IT company that develops and integrates industrial communication systems, automation solutions and dispatch software to improve operational communications and efficiency for enterprise clients worldwide.
### Responsibilities
- Designed reliable, secure, and efficient communication systems by applying telecommunications and computer engineering principles
- Planned and developed network layouts and infrastructures, ensuring compliance with client requirements and industry standards
- Produced detailed network diagrams, layouts, and technical drawings in **AutoCAD** to support project accuracy and implementation
- Leveraged the Structured Cabling System (SCS) plugin to streamline designs
## **Network Engineer** at JSC “ER-Telecom Holding” 
Mar 2012 - Feb 2014 (2 years)
[ER-Telecom Holding JSC](https://ertelecom.ru/en) provides broadband Internet, telephony, digital TV, Wi-Fi access, VPN and LoRaWAN services, as well as video surveillance solutions. 
### Responsibilities
- Administer and maintain main routers (Juniper) and switches (Cisco) in the ISP’s core data center. Monitor **VLAN** plans and ensure correct **QinQ** implementation for network segmentation
- Deploy and maintain major backbone network nodes for the ISP:  
	- Configure aggregation-level network equipment to ensure stable and efficient traffic flow
	- Set up industrial **MOXA** and **ZTE** switches for system monitoring of the nodes.
	- Install cellular modems (**MOXA**) to provide backup connectivity for backbone nodes
- Configure and troubleshoot last-mile switches (**Cisco,D-Link, ZTE**):  
	- Set up switches to participate in **RSTP** rings for network redundancy  
	- Troubleshoot connectivity and performance issues using Link Layer Discovery Protocol (**LLDP**)
	- Monitor **VLAN** plans and ensure correct **QinQ** implementation for network segmentation
- Monitor 48V power system (Delta inverters and batteries) to ensure stable power supply for all devices in the core data center
- Maintain Dell and HP servers, including upgrading/replacing HDDs, RAM, processors, and power supplies
- Monitor network performance (**SNMP**), availability, and security, responding to incidents promptly
- Provide technical support to users and clients, ensuring minimal downtime and optimal service quality
### Project
#### ISP Network Deployment
Participated in the construction and deployment of the internet service provider (ISP) network for the city of Tomsk (population ~600,000), including installation, configuration, and integration of network equipment to ensure reliable connectivity and service delivery across the urban area.
## **System Administrator** at Television and Radio Broadcasting Company "Tomsk"
Sep 2010 - Mar 2012 (1 year 7 months)
[GTRK](https://www.tvtomsk.ru/) A regional television and radio broadcasting company providing audiovisual content and media in Tomsk.
### Responsibilities
• Maintain the organisation’s IT infrastructure, ensuring security, reliability, and high performance  
• Administer a Squid proxy server to optimise web traffic and enforce network access policies
• Manage **FreeBSD** and **Windows Server** environments  
• Administer **Active Directory**, including user accounts, group policies (GPO), permissions, and access control
• Provide technical support to end users, troubleshooting hardware, software, and network issues
### Project
#### Dalet System Deployment (News Production & Distribution system)
  Deployment of the [Dalet News Production & Distribution system](https://www.dalet.com/solutions/news-production/), involving requirements gathering, alignment with existing IT environments, and integration of broadcast infrastructure. Resolved issues related to partially deprecated legacy systems.
# Education
## Tomsk State University of Control Systems and Radioelectronics
Master of Engineering (Radio Engineering)
Sep 2005 - Aug 2010
## North Metropolitan TAFE
Diploma, Information Technology (Advanced Programming)
Feb 2026 - Jun 2027 (expected)
## North Metropolitan TAFE
Certificate IV, Information Technology (Programming)
Jul 2024 - Dec 2025
### TAFE Projects
#### WareLog Android App (.NET MAUI)
https://github.com/Dezkiy/WareLog
The application is a **warehouse tracking system** built with **.NET MAUI**. The client collects detailed goods information, including customer, receiver, and driver details, as well as images and signatures, and sends it to a centralized **PostgreSQL** database. The app also processes scanned QR-code items, matches them against a predefined database, and provides endpoints to handle scanned items. It generates output files for both matched and unmatched items using the **WareLog API**.

#### WareLog-API (fastAPI) 
https://github.com/Dezkiy/WareLog-API
WareLog API is a **FastAPI**-based application designed to process scanned QR code items and match them against a predefined database. It provides endpoints to handle scanned items, identify matches, and generate output files for both matched and unmatched items.
#### Web project (Tailwind CSS)

https://dezkiy.github.io/tafe_web_project/
Project using **JavaScript** and **Tailwind CSS** with a **mobile-first design**, integrating **API Ninjas** to fetch and display external data, implement dynamic content rendering, and enhance user interaction and responsiveness across devices.

# Licenses & certifications
## CKA: Certified Kubernetes Administrator
*Issued by Linux Foundation*
Jul 2024 - Jul 2026

[https://training.linuxfoundation.org/certification/verify/](https://training.linuxfoundation.org/certification/verify/)
LF-zasu7p5y5d
## AWS Certified Solutions Architect - Associate
*Issued by Amazon Web Services (AWS)* |
Apr 2024 - Apr 2027

[https://aws.amazon.com/verification](https://aws.amazon.com/verification)
43a1063551e74abea242ea184a34a813
## AWS Certified Cloud Practitioner
*Issued by Amazon Web Services (AWS)* |
Jan 2024 - Jan 2027

[https://aws.amazon.com/verification](https://aws.amazon.com/verification)
N0VD0MCDS1F41S9R
## Terraform Associate (HCTAO-003)
*Issued by HashiCorp* |
Aug 2024 - Aug 2026

https://www.credly.com/earner/earned/badge/564ea852-218a-4ff7-91fc-1695bd638d69
HCP00217565
## Python Network Programming for Network Engineers
*Issued by Udemy*
Apr 2020 - Current

[https://www.udemy.com/certificate/UC-beb59de9-cc1a-4f93-918b-30d1e5029593/](https://www.udemy.com/certificate/UC-beb59de9-cc1a-4f93-918b-30d1e5029593/)
## Remote Pilot Licence (RePL)
*Issued by CASA* |
Aug 2025 - Current

## Python 3 Tutorial course
*Issued by SoloLearn* |
Mar 2018 - Current

https://www.sololearn.com/Certificate/1073-4033838/pdf/  
## Huawei Certification Routing & Switching (HCNA-R&S)
*Issued by Huawei Technologies* |
Dec 2018 - Current
## Interconnecting Cisco Network Devices Part 2 (ICND2)
*Issued by CISCO* | 
Sep 2017 - Current
## Game Theory (mathematics of strategy and rational decision-making)
*Issued by Higher School of Economics (Coursera)* | 
Jan 2017 - Current

[https://www.coursera.org/account/accomplishments/verify/K2KBT39K9KC7](https://www.coursera.org/account/accomplishments/verify/K2KBT39K9KC7)
# Additional
- Available **upon request**
## Interests/Hobbies
- Internet of Things (IoT), Home Assistant, 
- Surfing, Snowboarding, Playing guitar
