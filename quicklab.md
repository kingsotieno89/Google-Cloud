
## 🚀 Implement Load Balancing on Compute Engine: Challenge Lab | [GSP313](https://www.cloudskillsboost.google/focuses/10258?parent=catalog)



**Launch Cloud Shell:**
Start your Google CloudShell session by [clicking here](https://console.cloud.google.com/home/dashboard?project=&pli=1&cloudshell=true).


```bash
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/Implement%20Load%20Balancing%20on%20Compute%20Engine%20Challenge%20Lab/quicklabgsp313.sh
sudo chmod +x quicklabgsp313.sh
./quicklabgsp313.sh
```
- This command downloads the setup script from GitHub. The script will help configure the environment and perform necessary setup steps.

### Lab might task 10 - 15 mintues to updated the score so don't worry!

Implement Load Balancing on Compute Engine: Challenge Lab

This script will help achieve the following
Create an instance.
Create an HTTP load balancer in front of two web servers.



Task 1. 
Create a project jumphost instance

Task 2. 
Set up an HTTP load balancer
You will serve the site via nginx web servers, but you want to ensure that the environment is fault-tolerant. Create an HTTP load balancer with a managed instance group of 2 nginx web servers. 

The Steps are as follows:
Create an instance template. Don't use the default machine type. Make sure you specify e2-medium as the machine type and create the Global template.
Create a managed instance group based on the template.
Create a firewall rule named as Firewall rule to allow traffic (80/tcp).
Create a health check.
Create a backend service and add your instance group as the backend to the backend service group with named port (http:80).
Create a URL map, and target the HTTP proxy to route the incoming requests to the default backend service.
Create a target HTTP proxy to route requests to your URL map
Create a forwarding rule.
