---
layout: post
title:  "SimpleRisk"
date:   2024-06-28 12:11:42 -0700
categories: Security
---
    Post category:Security / Technology

<a href="https://www.simplerisk.com">https://www.simplerisk.com</a>

SimpleRisk is a comprehensive GRC platform that can be used for all of your Governance, Risk Management and Compliance needs. It boasts functionality that is comprehensive enough to be utilized by some of the largest organizations on the planet while presenting a user interface that is so simple and intuitive it can be used by the least technical people in your organization.
Option 1: SimpleRisk Scripted Installation

Run this command as “root” on a newly provisioned system to perform a scripted SimpleRisk installation:

curl -sL https://raw.githubusercontent.com/simplerisk/setup-scripts/master/simplerisk-setup.sh | bash -

Currently supported Operating Systems include:

    Ubuntu 22.04
    Ubuntu 20.04
    CentOS 8
    CentOS 7
    SLES 15
    RHEL 9
    RHEL 8
    Debian 11

Option 2: SimpleRisk Virtual Machine Installation
VMWare Virtual Machine
1) Download the Virtual Machine Image:

SIMPLERISK 20240318-001 VIRTUAL MACHINE (VMWare)
2) Validate the Checksum:

MD5 Checksum = 20a97717982c3116db57d37319a30ee0
3) Install the Virtual Machine:

INSTALL SIMPLERISK AS A VMWARE APPLIANCE
4) Secure the Virtual Machine:

SECURE YOUR SIMPLERISK VIRTUAL MACHINE
VirtualBox Virtual Machine
1) Download the Virtual Machine Image:

SIMPLERISK 20240318-001 VIRTUAL MACHINE (Virtualbox)
2) Validate the Checksum:

MD5 Checksum = f5a825f8d186e3c38e7edb7b3730d1f5
3) Install the Virtual Machine:

INSTALL SIMPLERISK AS A VIRTUALBOX APPLIANCE
4) Secure the Virtual Machine:

SECURE YOUR SIMPLERISK VIRTUAL MACHINE

Option 3: SimpleRisk Docker Installation
DockerHub Image
1) Download the SimpleRisk image from DockerHub:

docker pull simplerisk/simplerisk
2) Start the Docker Container:

docker run –name simplerisk -d -p 80:80 -p 443:443 simplerisk/simplerisk
3) Test Your SimpleRisk Instance:

https://localhost

Compiled Docker Image
1) Clone the SimpleRisk Docker Repository:

git clone https://github.com/simplerisk/docker.git simplerisk-docker
2) Change to the Docker directory:

cd simplerisk-docker/simplerisk
3) Build the SimpleRisk Docker Image:

docker build -t simplerisk/simplerisk -f bionic/Dockerfile .
4) Start the Docker Container:

docker run –name simplerisk -d -p 80:80 -p 443:443 simplerisk/simplerisk
5) Test Your SimpleRisk Instance:

https://localhost

