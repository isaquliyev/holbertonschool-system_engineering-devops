# 2. Secured and monitored web infrastructure

<p align="center"><img src="https://github.com/isaquliyev/holbertonschool-system_engineering-devops/blob/master/web_infrastructure_design/task_2.png"></p>

## Infrastructure Components:

### SSL (Secure Sockets Layer):
SSL is a cryptographic protocol designed to secure communication over computer networks, particularly the internet. It encrypts data exchanged between clients (e.g., web browsers) and servers, preventing interception or tampering by malicious parties. SSL is widely used to secure sensitive information like login credentials and payment details. Websites using SSL are accessed over HTTPS, signifying an encrypted and secure connection. SSL certificates, issued by trusted Certificate Authorities (CAs), authenticate website identities, establishing secure connections between clients and servers.

### Firewall:
A firewall is a network security device or software that monitors and controls incoming and outgoing network traffic based on predetermined security rules. Serving as a barrier between trusted internal networks and untrusted external networks, firewalls filter traffic to prevent unauthorized access, attacks, and data breaches. Firewalls can be hardware-based, software-based, or a combination. They inspect data packets, enforcing rules based on factors such as IP addresses, ports, protocols, and application types. Firewalls may include features like intrusion detection, virtual private network (VPN) support, and deep packet inspection.

### Web Server QPS Monitoring:
Monitoring web server Queries Per Second (QPS) involves tracking the rate at which the server receives and processes client requests. QPS monitoring is crucial for assessing performance, identifying bottlenecks, and ensuring the server handles workloads without issues. Monitoring tools collect metrics like request rates, response times, error rates, and resource utilization to provide insights for optimization, resource scaling, and issue troubleshooting.

## Infrastructure Issues:

### Terminating SSL at the Load Balancer Level:
- **Risk of Decrypted Traffic Exposure:** Terminating SSL at the load balancer exposes decrypted traffic between the load balancer and backend servers, potentially compromising security.
- **Loss of Client Certificate Visibility:** Backend servers lose visibility of client certificates, potentially affecting authentication or authorization processes.

### Single MySQL Server Handling Writes:
- **Single Point of Failure:** Relying on one MySQL server for write operations creates a single point of failure, risking data loss or service disruption if the server fails.
- **Scalability Limitations:** Limited scalability as only one server manages write operations, potentially causing performance issues during heavy loads.

### Servers with Identical Components:
- **Increased Vulnerability:** Having identical components across servers increases vulnerability to system-wide issues if a critical vulnerability affects a shared component.
- **Scalability and Flexibility Limitations:** Limits scalability and flexibility as different components may have varied resource requirements, hindering adaptability to changing workloads.
