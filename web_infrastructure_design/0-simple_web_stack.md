# 0. Simple Web Stack

<p align="center"><img src="https://github.com/isaquliyev/holbertonschool-system_engineering-devops/blob/main/web_infrastructure_design/task_0.png"></p>

##Infrastructure Specifics:


### Definition of a Server:
A server, in the context of computer systems, refers to a program or device that offers services to other programs (clients) and their users. It can be a physical machine or a virtual one within a data center. Servers, in the client/server model, respond to and fulfill requests from client programs, which may run on the same or different computers. The term "server" can encompass physical machines, virtual machines, or software providing server services, and its functionality varies based on its usage.

### Role of Domain Names:
Domain names act as internet navigational addresses, similar to street names, while IP addresses pinpoint actual locations. The Domain Name System (DNS) translates complex IP addresses into memorable letter strings, simplifying internet navigation. Hierarchically organized, domain names include top-level domains (TLDs) like .com and .org, country code top-level domains (ccTLDs) such as .fr or .au, and subdomains that further delineate the hierarchy. Domain names enhance internet accessibility and usability compared to IP addresses.

### DNS Record for "www.foobar.com":
The "www" in "www.foobar.com" typically corresponds to a DNS record known as a "CNAME" (Canonical Name) record. This CNAME record associates the hostname "www" with the domain name "foobar.com," acting as an alias and directing traffic intended for "www.foobar.com" to the same location as "foobar.com."

### Role of Web Server:
A web server processes end user requests made through a web browser. Communication between the web server (or browser) and the user occurs via Hypertext Transfer Protocol (HTTP). The primary function of a web server is to store, process, and deliver requested information or webpages to end users.

### Role of Application Server:
An application server serves as middleware between the operating system and external resources, hosting user business logic and ensuring accessibility and performance. Despite challenges like variable client traffic and hardware failures, the application server ensures the smooth functioning of business applications.

### Role of Database:
Databases play a crucial role in web application development by storing and organizing data essential for functionality. They act as repositories for various information, such as product details and customer information. Understanding databases is vital for comprehending web application intricacies, facilitating seamless interaction between the application and its data.

### Server Communication with User's Computer:
When a user requests a website, the server communicates with the user's computer using Hypertext Transfer Protocol (HTTP) or its secure variant, HTTPS. These protocols define rules for information exchange between the server and the user's browser, allowing the server to process requests and send back the requested web page or resources.

## Infrastructure Issues:


### Single Point of Failure (SPOF):
SPOF, or "Single Point of Failure," refers to a component within a system, such as a server or network device, whose failure could lead to the entire system becoming unavailable. Identifying and mitigating SPOFs is crucial for ensuring high availability and reliability. Redundancy, failover mechanisms, and disaster recovery plans are implemented to address SPOFs and minimize their impact.

### Downtime During Maintenance:
"Downtime" in IT refers to periods when a system is unavailable. Maintenance downtime occurs when a machine is non-operational due to required maintenance work. Planning and managing maintenance activities are essential to minimize the impact of downtime on system operations.

### Scalability Challenges with High Traffic:
The ability to scale infrastructure is crucial to accommodate increased website traffic. Without proper scalability measures, websites may experience performance issues or crashes during peak traffic, leading to lost visitors and revenue. Implementing scalability ensures website responsiveness and reliability even under heavy traffic, preserving performance and user experience.
