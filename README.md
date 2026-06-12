# Task 1 - Launch a Virtual Machine on AWS EC2

## Objective
Launch an Ubuntu EC2 instance and configure a web server.

## Tools Used
- AWS EC2
- Ubuntu 24.04 LTS
- Apache2 Web Server

## Steps Performed
1. Created an AWS EC2 instance.
2. Selected Ubuntu Server 24.04.
3. Used t3.micro instance type.
4. Connected using EC2 Instance Connect.
5. Updated packages.
6. Installed Apache2.
7. Verified Apache service status.
8. Accessed the web server using the public IP.

## Commands Used

```bash
sudo apt update
sudo apt install apache2 -y
systemctl status apache2
```

## Public IP

13.61.141.54

## Result

Successfully launched a virtual machine on AWS and hosted the Apache2 default webpage.
