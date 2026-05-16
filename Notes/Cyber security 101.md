 - cryptographic method or product considered bogus or fraudulent- snake oil.
 - **socket statitics(ss)** command replace for netstat in linux.
 - **Shodan**, a search engine for devices connected to the Internet. It allows you to search for specific types and versions of servers, networking equipment, industrial control systems, and IoT devices.
 - **Censys**, on the other hand, focuses on Internet-connected hosts, websites, certificates, and other Internet assets. 
 - **VirusTotal** is an online website that provides a virus-scanning service for files using multiple antivirus engines.
 - **Have I Been Pwned (HIBP)** does one thing; it tells you if an email address has appeared in a leaked data breach.
 - **https://www.nist.gov/**- quantum computing.
 - For more information and to search for existing CVEs, visit the CVE Program website. Alternatively, visit the National Vulnerability Database (NVD) website. 
 - https://www.exploit-db.com/ -exploit database site and GITHUB.
 - **Offensive Security**: It is an approach to find possible security threats by exploiting the system . dirb is the command to check the hidden urls. syn : dirb url.
- ##**Defensive Security**: Also knowns as blue team.  - 1: Monitoring and Detecting : continuously observing network and system activity to detect suspicious behaviour. - 2: Incidence Response : Containing and removing threats and restoring business normally. - 3. Threat Intelligence : Gathering and using information about attackers—their latest methods, targets, and trends—can greatly strengthen an organisation’s defences. - 4. Vulnerability Management: fixing system and software flaws to avoid/lower threats . - 5. Investigation and analysis : members of the teams always monitoring and analysing whats happening inside the organisation. - **Defensive Measures** : Employee training, IDS( Intrusion detection system) : Acts like surveillance camera. Monitor and alert when suspicios activity occured. Firewall, Security policies. 
- SIEMs (Security Information and Event Management) systems are the central place for all data and information collected from security devices, workstations, servers, and more within an organisation.
- A VLAN (Virtual Local Area Network) is a way to divide one physical network into multiple logical networks. It helps organize and secure devices even if they are connected to the same switch.
- Router at layer 3 of OSI model and switch  at layer2 of OSI model.
- A VPN (Virtual Private Network) creates a secure encrypted tunnel between your device and another network over the internet.
- A firewall is a security system that controls network traffic based on rules. The key difference between stateful and stateless firewalls is how they track connections. A stateless firewall treats each packet independently, without remembering anything about previous packets. A stateful firewall keeps track of active connections and makes decisions based on the state of the connection.
- User opens website
        ↓
Internet
        ↓
Company Router
        ↓
Port forwarding rule
        ↓
Internal Web Server
- Port forwarding = router sending internet traffic to a specific device inside local network.
- Roouter forwards the packet containing IP address and data. Switch adds mac address to the  packet (frame ) and forward it to right PC.
- Handshake process - syn-ack/syn-ack-fin.
- gTLD- Generic top level domain -.com, .ed etc. ccTLD-Country code top level domain - .ca, .co.uk etc.
- Second Level Domain - eg tryhackme.com - tryhackme is the second level domain . Second level domain+TLD . Can use a-z 0-9 and hyphen.Limit -63 characters.
- admin.tryhackme.com - admin is the subdomain. 63 characters limit and 253 characters in length.
- A DNS record tells: where a website/server is located, which mail server to use, which services belong to a domain. 
- | Record Type| Purpose |
  | ----------- |------- |
  | A | Domain → IPv4 |
  | AAAA | Domain → IPv6 |
  | CNAME | Alias to another domain |
  | MX | Mail server |
  | NS | Name server |
  | PTR | IP → Domain |
  | TXT | Text/security info |

- **Why DNS Records Matter in Cybersecurity**

- SOC Analysts often investigate:
- malicious domains
- suspicious DNS traffic
- phishing domains
- SPF/DKIM issues
- DNS tunneling attacks

- **Why DNS Requests Matter in Cybersecurity**

SOC Analysts monitor DNS requests because attackers may use:
- malicious domains
- phishing websites
- DNS tunneling
-malware communication

Suspicious DNS traffic is a very common investigation area in SOC roles.


-Browser
   ↓
Local Cache
   ↓
DNS Resolver
   ↓
Root Server
   ↓
TLD Server (.com)
   ↓
Authoritative DNS Server
   ↓
IP Address Returned
   ↓
Browser Opens Website

- A hypervisor is the core technology behind virtualization. It's the software that creates and manages virtual machines.
- An HTTP status code is a number sent by a web server to tell the client (browser/app) what happened with the request. When your browser requests a webpage, the server responds with: data/content and a status code.
- 🔹 Common HTTP Status Codes
✅ 200 OK

Request successful.

Website loaded properly.

🔀 301 Moved Permanently

Website/page moved to another URL.

Browser gets redirected automatically.

❌ 400 Bad Request

The request was invalid.

🔒 401 Unauthorized

Login/authentication required.

🚫 403 Forbidden

Server understood request but refuses access.

🔍 404 Not Found

Page does not exist.

Very common error.

⚠️ 500 Internal Server Error

Problem occurred on the server side.

🔧 503 Service Unavailable

Server temporarily unavailable or overloaded.

- 🔁 **Status Code Categories Range	Meaning**
- 1xx	Informational
- 2xx	Success
- 3xx	Redirection
- 4xx	Client errors
- 5xx	Server errors

- **Why Status Codes Matter in Cybersecurity**

SOC Analysts and security teams monitor status codes because:

many 401/403 errors may indicate attack attempts
repeated 404 requests may indicate scanning
500 errors may reveal server problems

Attackers often generate suspicious HTTP responses during reconnaissance.



