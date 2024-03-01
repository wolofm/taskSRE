# taskSRE
Name : Bouabsa Abdel


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





