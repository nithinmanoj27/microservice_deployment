# Microservice Deployment on VirtualBox VMs

This repository contains a simple Node.js microservice application that can be deployed on VirtualBox VMs.

## Prerequisites
1. VirtualBox installed on your host machine.
2. Ubuntu ISO downloaded and attached to the VMs.
3. Docker installed on both VMs.

## Steps to Deploy

### 1. Create Virtual Machines
- Create two VMs in VirtualBox (`VM1` and `VM2`).
- Install Ubuntu on both VMs.

### 2. Configure Network
- Set up a host-only network in VirtualBox.
- Assign static IPs to the VMs (e.g., `192.168.56.101` for VM1 and `192.168.56.102` for VM2).

### 3. Install Docker
On both VMs, run the following commands:
```bash
sudo apt update
sudo apt install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker
