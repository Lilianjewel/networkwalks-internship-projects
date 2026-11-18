# networkwalks-internship-projects week 2

WK2 PENTESTING PRORJECT AND REPORT 

In this week’s project, we were asked to Footprint 👣 using different tools and Scan using different Nmap-Zenmap.

I ran my Footprinting using theHarvester which was run using Kali Linux virtual machine, to collect publicly available information about the domain microsoft.com without interacting with the target directly. I first ran theHarvester -d microsoft.com -l 1000 -b baidu, which returned no IPs, emails, people or hosts. I then ran theHarvester -d microsoft.com -l 50 -b all to query every available source.
Many sources were skipped or failed because no API key was configured (for example Bevigil,and VirusTotal), and some returned errors (Chaos, Fofa, LeakIX, Robtex and ThreatCrowd). The results therefore come from the free sources only, such as Certspotter, and the Wayback Archive. With theHarvester I saw how many hosts, IPs, ASNs and emails turn up from public sources alone. 

I also ran footprinting for networkwalks.com using five Kali Linux tools. Whois, Nslookup, Whatweb, Curl, and Wafw00f. WHOIS gave me registration and name server details, WhatWeb identified the web technologies, Nslookup resolved the domain, Curl showed the HTTP headers, and Wafw00f detected the firewall. 

For the third activity, I used Zenmap to perform network discovery on my own local network on 11 November 2026 at 22:49. The goal was to identify live hosts together with their IP and MAC addresses. The main lesson is how much an attacker can learn before touching a system at all. Public records and ordinary network responses reveal a great deal when they are read carefully.
I also learned that findings only help when they are written up clearly: what was done, what was found, what it means, what risk it carries, and how to reduce that risk.

Lastly, all reconnaissance and scanning have to stay inside an authorized scope. This work was done as part of an educational lab.

NOTE: it is important to get autorizations to test before doing so.

Images of footprinting using multiple tools
<img width="638" height="356" alt="Screenshot 2026-11-12 3" src="https://github.com/user-attachments/assets/f03089c9-e31f-4110-bb19-7ca9014a5fca" />

<img width="637" height="368" alt="Screenshot 2026-11-12 212453" src="https://github.com/user-attachments/assets/53b127ff-4117-47fb-96a6-a952133f21c7" />

<img width="631" height="355" alt="Screenshot 2026-11-12 213333" src="https://github.com/user-attachments/assets/e75bb07b-2bb5-4f59-9737-20c78a715a73" />

Images of footprinting using theHarvester

<img width="633" height="385" alt="Screenshot 2026-11-12 204309" src="https://github.com/user-attachments/assets/c8ce449c-f525-4882-95ef-4de919763f3c" />

<img width="634" height="353" alt="Screenshot 2026-11-12 234740" src="https://github.com/user-attachments/assets/5bde983f-2389-41ad-b0c4-be8fff7d8c85" />

