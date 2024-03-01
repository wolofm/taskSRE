# taskSRE
Name : Bouabsa Abdel

Task #1 and #2
1. How would you structure your Terraform project if you have multiple environments
and use different cloud providers?
2. Write a Terraform script with the below requirements:
● Creates a ubuntu aws ec2-instance
● Install ansible
● Execute an ansible playbook (optional: Use Ansible script from Task #1 or any other )

*My answer :

I don't have much experience with Terraform so instead i'll combine the 2 tasks and proceed the way i know :

I did this on my Google Cloud existing Ubuntu instance.

$ sudo apt-add-repository ppa:ansible/ansible
Hit:1 http://europe-west1.gce.archive.ubuntu.com/ubuntu focal InRelease
Get:2 http://europe-west1.gce.archive.ubuntu.com/ubuntu focal-updates InRelease [114 kB]
Get:3 http://europe-west1.gce.archive.ubuntu.com/ubuntu focal-backports InRelease [108 kB]
Get:4 .....
Done

$ sudo apt update
Hit:1 http://europe-west1.gce.archive.ubuntu.com/ubuntu focal InRelease
Hit:2 http://europe-west1.gce.archive.ubuntu.com/ubuntu focal-updates InRelease
....

installing ansible and python 3

$ sudo apt install ansible

i believe from here i have to start and create ansible roles, then the database informations using MySQL DB, USER, PASSWORD.. and last step is writing the playbook with the database and app informations and run it


-
-
-
-
-
-
-


Task #3

If you have multiple Ubuntu prod instances, How would you monitor them? What would be your
monitoring strategy?

*My Answer for Task #3 : 

With multiple Ubuntu instances, setting up a monitoring strategy is crucial to ensure performance, and security

1- Centralized solution : 

A centralized monitoring solution that provides a dashboard for all instances. tool like Grafana with dashboard and widgets.

2- Alert System :

Set up alerts for critical issues before they impact the performance or availability of the instances.

Prometheus and Grafana can be used for this, these tools provide you the freedom to set up alert conditions, rules and notifications.

3- Testing :

performance testing to simulate various loads on the instances, using Apache jMeter for example, checking the Java version if available on the instance, installing Java if not installed, then jMeter wget (last version link...) setting up and make sure to avoid ineterferences with others services or softwares.

4- Optimization :

Review the monitoring setup to ensure it remains up to date and working smoothly, optimize monitoring tools and alerts according to the collected data

5- Documentation :

instances documentation for the monitoring setup. Including details about the what's being monitored, alerting configurations and tools, and any other processes. this documentation is important for all new team members for ensuring consistency in monitoring exercices.

-
-
-
-
-
-



TASK 5 #

creating helm chat for wordpress 

$ mkdir wordpress-chart-task
$ cd wordpress-chart-task

nano values.yaml

inside indicate the website link and for wordpress

after create indication for Kubernetes manifests with the template and chart name including the IP, PORT and protocol for the connection

helm install, helm lint, and uninstall








