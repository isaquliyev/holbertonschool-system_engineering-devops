# 1. Distributed web infrastructure


<p align="center"><img src="https://github.com/isaquliyev/holbertonschool-system_engineering-devops/blob/master/web_infrastructure_design/task_1.png"></p>


## Infrastructure Components:


### Load Balancer:
A crucial component in ensuring high availability and reliability, a load balancer acts as a traffic manager, distributing incoming requests across multiple servers or resources. Its primary objectives include optimizing resource utilization, preventing individual servers from being overwhelmed, and ensuring an even workload distribution. Load balancers operate at different layers of the OSI model, such as Layer 4 (transport layer) and Layer 7 (application layer), offering varying levels of functionality and intelligence.

### Active-Passive Setup:
Also referred to as failover or standby configuration, an active-passive setup involves maintaining duplicate sets of resources, like servers or databases. The active set handles all incoming requests and data processing, while the passive set remains idle, ready to take over in case of a failure or outage. Continuous data replication from active to passive resources ensures synchronization and minimizes downtime during failover events.

### Integration of Load Balancer with Active-Passive Setup:
In an active-passive setup, the load balancer plays a crucial role in routing traffic to active resources while monitoring their health and availability. If active resources fail or become unresponsive, the load balancer, through health checks or monitoring probes, automatically redirects traffic to passive resources, ensuring transparent failover and continuous service availability with minimal disruption.

### Primary-Replica (Master-Slave) Cluster:
In this cluster, the primary node handles write requests, updating its data and replicating changes to replica nodes. Replica nodes maintain a copy of the data but handle only read queries, relying on replication from the primary node. The primary node manages writes, maintaining data integrity, while replica nodes serve as backups and manage read-heavy workloads. This setup ensures high availability, scalability, and fault tolerance for database systems.

## Infrastructure Issues:
Potential Single Point of Failure in Primary-Replica Cluster:
In a Primary-Replica cluster, the primary node poses a potential single point of failure. Measures such as redundancy and failover mechanisms should be implemented to mitigate this risk.

### Firewall Protection for Security:
Firewall protection is crucial for ensuring security by preventing unauthorized access and potential attacks. Configuring and maintaining firewalls is essential to safeguard the infrastructure.

### HTTPS for Secure Communication:
Implementing HTTPS is essential for secure communication, protecting data from interception during transit. This encryption protocol enhances the overall security posture of the infrastructure.

### Monitoring Tools for Early Issue Detection:
Monitoring tools play a vital role in detecting issues early, ensuring stability, security, and optimal performance. Regular monitoring helps identify potential problems and allows for timely intervention to maintain the integrity of the infrastructure.
