# Udacity-fullstack-project-final
Deploy the item catalog project ( https://github.com/stevelee87/Udacity-fullstack-project2 ) hosted in an AWS LightSail running Ubuntu and using PostgreSQL

## 1 Introduction

Please first refer to the Project 2 to understand how this web app works. This project is meant to focus only in to deploy this project 2 web app into the web using an AWS LightSail instance of Ubuntu 18.4 with the listed below requirements.

From Udacity's website:

### Project Overview
You will take a baseline installation of a Linux server and prepare it to host your web applications. You will secure your server from a number of attack vectors, install and configure a database server, and deploy one of your existing web applications onto it.

### Why this Project?
A deep understanding of exactly what your web applications are doing, how they are hosted, and the interactions between multiple systems are what define you as a Full Stack Web Developer. In this project, you’ll be responsible for turning a brand-new, bare bones, Linux server into the secure and efficient web application host your applications need.

### What will I Learn?
You will learn how to access, secure, and perform the initial configuration of a bare-bones Linux server. You will then learn how to install and configure a web and database server and actually host a web application.

## 2 General information

**Access**
Static IP: 3.84.131.65
Domain: http://www.estevamdonnabella.com

**SSH parameters:**
user: grader
port: 2200
How to connect: Dear Grader, please copy the public key code given at the udacity's project-submit field and create a `grader_id_rsa` file to paste the copied key into it. Create a hidden folder named `.ssh` into your home directory. Save the `grader_id_rsa.pub` key into this hidden folder. In your terminal, use the following command to connect via SSH: `ssh -i ~/.ssh/grader_id_rsa grader@3.84.131.65 -p 2200`. 

**Security**
* All the ports are bloqued with exception of: 80 (HTTP), 123 (NTP) and 2200 (SSH) both in Amazon console firewall and in Ubuntu ufw.
* The SSH port connection was changed from 22 (standard) to 2200.
* The SSH connection with password was desabled and it is possible to connect only with key pairs.
* The user _grader_ was given `sudo` access.
