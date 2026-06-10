# CloudVPN - WireGuard on AWS

## Overview

CloudVPN is a cloud-hosted VPN project built on AWS EC2 using Ubuntu Server and WireGuard.

The goal of this project is to provide secure remote access through an encrypted VPN tunnel while demonstrating AWS cloud infrastructure, Linux administration, networking, and security concepts.

---

## Technologies Used

* AWS EC2
* Ubuntu Server 26.04 LTS
* WireGuard
* Elastic IP
* AWS Security Groups
* SSH
* Linux

---

## Architecture

Client Device

↓

Internet

↓

AWS Elastic IP

↓

Ubuntu EC2 Instance

↓

WireGuard VPN Server

---

## Project Objectives

* Deploy a cloud-hosted VPN server
* Configure AWS networking components
* Implement secure remote administration using SSH
* Install and configure WireGuard VPN software
* Learn VPN deployment and network security fundamentals

---
![test](screenshots/Screenshot%202026-06-10%20145541.png)
## Phase 1 Completed

### EC2 Deployment

* Created Ubuntu EC2 instance
* Configured instance networking
* Assigned Elastic IP address

### Security Configuration

* Configured SSH access
* Configured UDP port 51820 for WireGuard traffic
* Created dedicated AWS Security Group

### Server Administration

* Connected to EC2 instance via SSH
* Updated Ubuntu packages
* Installed WireGuard VPN software

---

## Security Group Configuration

| Protocol | Port  | Purpose            |
| -------- | ----- | ------------------ |
| TCP      | 22    | SSH Administration |
| UDP      | 51820 | WireGuard VPN      |

---

## Screenshots

### EC2 Instance Running
![EC2 Instance](screenshots/Screenshot%202026-06-10%20145541.png)

### Security Group Configuration
![Security Group](screenshots/Screenshot%202026-06-10%20145614.png)

### WireGuard Installation Verification
![WireGuard](screenshots/Screenshot%202026-06-10%20144126.png)



---

## Future Improvements

* Generate WireGuard public/private keys
* Configure WireGuard server
* Configure VPN client devices
* Validate encrypted VPN connectivity
* Support multiple VPN clients
* Automate deployment using Terraform

---

## Skills Demonstrated

* AWS Cloud Infrastructure
* Linux Administration
* VPN Technologies
* Network Security
* Security Group Management
* SSH Remote Administration
* Cloud Networking
* Infrastructure Deployment

---

## Lessons Learned

This project provided hands-on experience with AWS networking, Linux server administration, EC2 deployment, security group management, WireGuard installation, and VPN infrastructure design.

