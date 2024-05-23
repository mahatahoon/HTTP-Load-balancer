
# Load Balancer Setup with Nginx and Apache HTTPD

This repository contains a Bash script that sets up a load balancer using Nginx and installs Apache HTTPD on multiple servers. The load balancer distributes incoming requests across the HTTPD servers, improving performance and reliability.

## Prerequisites

Before running the script, ensure the following:

1. You have SSH access to the target servers (VM1, VM2, and VM3).
2. Replace the placeholders (`$1`, `$2`, and `$3`) in the script with actual server hostnames or IP addresses.

## Usage

1. Clone this repository to your local machine.
2. Make the script executable: `chmod +x LoadBalancerScript.sh`.
3. Execute the script, passing the server information as arguments:
   ```bash
   ./LoadBalancerScript.sh VM1_HOST VM2_HOST VM3_HOST

- The script will:
    - Install Nginx on VM1.
    - Install Apache HTTPD on VM2 and VM3.
    - Configure Nginx as a load balancer, forwarding requests to the HTTPD servers.
    - Restart Nginx to apply the changes.


Remember to replace the placeholders (`VM1_HOST`, `VM2_HOST`, and `VM3_HOST`) with the actual server IP Adresses. 

