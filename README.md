##Prometheus

Prometheus, at its core, is a very simple and powerful tool to monitor and track your servers. Let’s take a use case. A company deploys and services 100s of ec2 instances on Amazon. How will that company be able to keep track of all the events and services that are running on those instances? What if one of those instances seem fine and is up and running, however, the core service it is meant for has crashed. The only way to check this is through the log files, but who will be responsible for checking through the log files of hundreds of instances?

This is where a service like Prometheus is so useful. Prometheus can monitor hundreds of instances and display metrics and statistics from all of them to you in one simple dashboard. You can even get more in-depth dashboards by connecting Grafana to your Prometheus service.

Grafana is a web application that gives you visualization tools. In a nutshell, you can create and use dashboards from Grafana to visualize all the statistics and metrics presented by Prometheus.

# Project Scope
Today we will be creating an Ansible playbook to automate the creation of an EC2 instance as well as the download of grafana, node_exporter, and Prometheus into that instance. We will tackle this project in small steps.

##Step 1
Manually create an ec2 box and download Prometheus, node_exporter, and grafana into and ensure everything is running.

Step 2
Create an Ansible playbook that will go through that same process in step 1.

Step 3
Write into the playbook the ability to create an ec2 instance.

End
With the run of a single playbook, an ec2 instance should be deployed with Prometheus, node_exporter, and grafana installed into it.

