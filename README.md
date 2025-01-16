Implement Load Balancing on Compute Engine: Challenge Lab

This script
Task 1. Create a project jumphost instance

Task 2. Set up an HTTP load balancer
You will serve the site via nginx web servers, but you want to ensure that the environment is fault-tolerant. Create an HTTP load balancer with a managed instance group of 2 nginx web servers. 

The Steps 

Create an instance template. Don't use the default machine type. Make sure you specify e2-medium as the machine type and create the Global template.
Create a managed instance group based on the template.
Create a firewall rule named as Firewall rule to allow traffic (80/tcp).
Create a health check.
Create a backend service and add your instance group as the backend to the backend service group with named port (http:80).
Create a URL map, and target the HTTP proxy to route the incoming requests to the default backend service.
Create a target HTTP proxy to route requests to your URL map
Create a forwarding rule.
