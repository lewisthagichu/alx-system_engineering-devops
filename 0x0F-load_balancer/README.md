# 0x0F. Load balancer
## Overview
In continuation of the web server configuration initiated in Project 0x0B, two additional servers have been introduced to enhance the infrastructure. The first server replicates the Nginx configuration of the original server, while the second server is designated for setting up an HAproxy load balancer. This load balancer efficiently manages both web servers, ensuring optimal distribution of incoming requests.

# Implementation Specifications
## Tasks 📃
### 0. Double the Number of Webservers
To scale the web server infrastructure, the number of webservers has been doubled. This involves replicating the Nginx configuration on a new server.

#### Task Details:
**File:** 0-custom_http_response_header
**Description:** Bash script that installs and configures Nginx on a server with a custom HTTP response header.

* The name of the HTTP header is X-Served-By.
* The value of the HTTP header is the hostname of the server.
### 1. Install Your Load Balancer
The introduction of an HAproxy version 1.5 load balancer is crucial for efficient distribution of incoming requests among the web servers.

#### Task Details:
**File:** 1-install_load_balancer
**Description:** Bash script that installs and configures HAproxy version 1.5 on a server.

* Enables management via the init script.
* Requests are distributed using a round-robin algorithm.
### 2. Puppet Custom HTTP Response Header
Automation of the task of creating a custom HTTP header response has been implemented using Puppet on the Nginx server.

#### Task Details:
**File:** 2-puppet_custom_http_response_header.pp
**Description:** Bash script that, similar to Task #0, automates the creation of a custom HTTP header response using Puppet.

* The name of the custom HTTP header is X-Served-By.
* The value of the custom HTTP header is the hostname of the server Nginx is running on.
