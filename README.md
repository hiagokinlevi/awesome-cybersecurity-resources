# Awesome Cybersecurity Resources [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, platforms, and learning material for network security, penetration testing, and blue team / defensive security.

[![GitHub stars](https://img.shields.io/github/stars/adifreza/awesome-cybersecurity-resources?style=flat)](https://github.com/adifreza/awesome-cybersecurity-resources/stargazers)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)

This list is maintained by an Informatics student specializing in network security. It focuses on the day-to-day toolkit of a network defender and tester: scanning and reconnaissance, vulnerability assessment, offensive frameworks, traffic analysis, detection engineering, and the study material needed to build the underlying skills. Every entry links to a real, actively maintained project or a well-known learning resource.

## Contents

- [Network Scanning & Reconnaissance](#network-scanning--reconnaissance)
- [Vulnerability Assessment](#vulnerability-assessment)
- [Penetration Testing Frameworks](#penetration-testing-frameworks)
- [Wireless Security](#wireless-security)
- [Traffic Analysis & Packet Sniffing](#traffic-analysis--packet-sniffing)
- [Intrusion Detection / Prevention (IDS/IPS)](#intrusion-detection--prevention-idsips)
- [Log Analysis & SIEM](#log-analysis--siem)
- [OSINT Tools](#osint-tools)
- [CTF Practice Platforms](#ctf-practice-platforms)
- [Vulnerable Apps for Practice](#vulnerable-apps-for-practice)
- [Certifications](#certifications)
- [Cheat Sheets](#cheat-sheets)
- [Blogs & Newsletters](#blogs--newsletters)
- [YouTube Channels & Podcasts](#youtube-channels--podcasts)
- [Books](#books)

## Network Scanning & Reconnaissance

- [Nmap](https://nmap.org) - The de facto standard for host discovery, port scanning, and service/OS fingerprinting.
- [Masscan](https://github.com/robertdavidgraham/masscan) - Asynchronous TCP port scanner able to sweep the entire internet in minutes.
- [RustScan](https://github.com/RustScan/RustScan) - Fast port scanner that pipes open ports straight into Nmap for deeper analysis.
- [OWASP Amass](https://github.com/owasp-amass/amass) - In-depth attack surface mapping and external asset discovery via DNS enumeration.
- [Recon-ng](https://github.com/lanmaster53/recon-ng) - Modular reconnaissance framework with a Metasploit-like workflow for web-based OSINT.
- [theHarvester](https://github.com/laramies/theHarvester) - Gathers emails, subdomains, hosts, and names from public sources.
- [dnsrecon](https://github.com/darkoperator/dnsrecon) - DNS enumeration script for zone transfers, brute forcing, and record analysis.
- [Netdiscover](https://github.com/netdiscover-scanner/netdiscover) - Active/passive ARP reconnaissance tool for mapping hosts on a local network.
- [fierce](https://github.com/mschwager/fierce) - DNS reconnaissance tool for locating non-contiguous IP space and hostnames.

## Vulnerability Assessment

- [OpenVAS / Greenbone Community Edition](https://www.greenbone.net/en/community-edition/) - Full-featured open-source vulnerability scanner and management platform.
- [Nessus](https://www.tenable.com/products/nessus) - Widely used commercial vulnerability scanner with a free tier for home use.
- [Nuclei](https://github.com/projectdiscovery/nuclei) - Template-based vulnerability scanner driven by a large community rule set.
- [Nikto](https://github.com/sullo/nikto) - Web server scanner that checks for dangerous files, outdated software, and misconfigurations.
- [OWASP ZAP](https://www.zaproxy.org) - Open-source web application security scanner and intercepting proxy.
- [Trivy](https://github.com/aquasecurity/trivy) - Scanner for vulnerabilities in containers, filesystems, and infrastructure as code.
- [Vuls](https://github.com/future-architect/vuls) - Agentless vulnerability scanner for Linux, FreeBSD, and cloud hosts.
- [Wapiti](https://github.com/wapiti-scanner/wapiti) - Black-box web application vulnerability scanner that audits by fuzzing.
- [Rapid7 InsightVM / Nexpose](https://www.rapid7.com/products/insightvm/) - Commercial vulnerability management with live risk scoring.

## Penetration Testing Frameworks

- [Metasploit Framework](https://github.com/rapid7/metasploit-framework) - The most widely used exploitation and post-exploitation framework.
- [Kali Linux](https://www.kali.org) - Debian-based distribution bundling hundreds of preconfigured security tools.
- [Impacket](https://github.com/fortra/impacket) - Python classes for crafting and manipulating network protocols, core to many AD attacks.
- [Sliver](https://github.com/BishopFox/sliver) - Open-source cross-platform adversary emulation and command-and-control framework.
- [PowerShell Empire](https://github.com/BC-SECURITY/Empire) - Post-exploitation framework with encrypted C2 for Windows, Linux, and macOS.
- [Covenant](https://github.com/cobbr/Covenant) - .NET command-and-control framework with a collaborative web interface.
- [Havoc](https://github.com/HavocFramework/Havoc) - Modern, modular post-exploitation command-and-control framework.
- [BeEF](https://github.com/beefproject/beef) - Browser Exploitation Framework focused on client-side attack vectors.
- [Villain](https://github.com/t3l3machus/Villain) - Backdoor generator and multi-session shell handler with peer-linking.

## Wireless Security

- [Aircrack-ng](https://www.aircrack-ng.org) - Complete suite for monitoring, attacking, testing, and cracking Wi-Fi networks.
- [Wifite2](https://github.com/kimocoder/wifite2) - Automated wireless auditing tool that wraps the aircrack-ng suite and hcxtools.
- [Kismet](https://www.kismetwireless.net) - Wireless network and device detector, sniffer, wardriving tool, and IDS.
- [Bettercap](https://www.bettercap.org) - Swiss-army knife for network attacks and monitoring, including Wi-Fi and BLE.
- [Reaver](https://github.com/t6x/reaver-wps-fork-t6x) - Brute-force attack against Wi-Fi Protected Setup (WPS) registrar PINs.
- [hcxdumptool](https://github.com/ZerBea/hcxdumptool) - Captures packets from WLAN devices for offline PMKID/handshake cracking.
- [Wifiphisher](https://github.com/wifiphisher/wifiphisher) - Rogue access point framework for red team Wi-Fi phishing assessments.
- [airgeddon](https://github.com/v1s1t0r1sh3r3/airgeddon) - Multi-use bash script that automates common wireless attack workflows.
- [Fluxion](https://github.com/FluxionNetwork/fluxion) - Social-engineering evil-twin attack framework for recovering WPA/WPA2 keys.

## Traffic Analysis & Packet Sniffing

- [Wireshark](https://www.wireshark.org) - The reference graphical network protocol analyzer.
- [tcpdump](https://www.tcpdump.org) - Command-line packet capture built on libpcap, available almost everywhere.
- [Zeek](https://zeek.org) - Network analysis framework that turns traffic into high-level structured logs.
- [Arkime](https://arkime.com) - Large-scale, open-source full packet capture, indexing, and search system.
- [NetworkMiner](https://www.netresec.com/?page=NetworkMiner) - Network forensic analysis tool for extracting files and credentials from PCAPs.
- [Scapy](https://scapy.net) - Python library for crafting, sending, sniffing, and dissecting packets.
- [mitmproxy](https://mitmproxy.org) - Interactive HTTPS proxy for intercepting, inspecting, and modifying traffic.
- [ngrep](https://github.com/jpr5/ngrep) - A grep-like utility that applies pattern matching to live network packets.
- [termshark](https://github.com/gcla/termshark) - Terminal user interface for tshark, inspired by Wireshark.

## Intrusion Detection / Prevention (IDS/IPS)

- [Snort](https://www.snort.org) - Long-standing signature-based network intrusion detection and prevention system.
- [Suricata](https://suricata.io) - High-performance, multi-threaded IDS/IPS and network security monitoring engine.
- [SELKS](https://github.com/StamusNetworks/SELKS) - Ready-to-use Suricata-based IDS/IPS and network security monitoring platform.
- [CrowdSec](https://github.com/crowdsecurity/crowdsec) - Collaborative, behavior-based intrusion prevention with a crowd-sourced blocklist.
- [OSSEC](https://www.ossec.net) - Host-based intrusion detection with log analysis, rootkit detection, and alerting.
- [Security Onion](https://securityonionsolutions.com) - Free Linux distro for threat hunting, monitoring, and log management.
- [Fail2ban](https://github.com/fail2ban/fail2ban) - Scans log files and bans IPs showing malicious signs such as brute-force attempts.
- [Maltrail](https://github.com/stamparm/maltrail) - Malicious traffic detection system using public blacklists and heuristics.
- [Sagan](https://github.com/quadrantsec/sagan) - Real-time log analysis and correlation engine with a Snort-like rule syntax.

## Log Analysis & SIEM

- [Elastic Stack (ELK)](https://www.elastic.co/elastic-stack) - Elasticsearch, Logstash, and Kibana for ingesting, searching, and visualizing logs.
- [Wazuh](https://wazuh.com) - Unified XDR and SIEM platform combining endpoint telemetry with log correlation.
- [Graylog](https://graylog.org) - Centralized log management with alerting, dashboards, and a query language.
- [Splunk Free](https://www.splunk.com/en_us/download/splunk-enterprise.html) - Industry-standard data platform for security analytics, free up to a daily volume limit.
- [Sigma](https://github.com/SigmaHQ/sigma) - Generic, shareable signature format for SIEM detection rules.
- [TheHive](https://github.com/TheHive-Project/TheHive) - Scalable security incident response platform for SOC collaboration.
- [Grafana Loki](https://grafana.com/oss/loki/) - Horizontally scalable log aggregation system inspired by Prometheus.
- [AlienVault OSSIM](https://cybersecurity.att.com/products/ossim) - Open-source SIEM bundling asset discovery, IDS, and event correlation.
- [HELK](https://github.com/Cyb3rWard0g/HELK) - Hunting ELK platform with analytics and Jupyter notebooks for threat hunting.

## OSINT Tools

- [Maltego](https://www.maltego.com) - Graph-based link analysis tool for mapping relationships between entities.
- [SpiderFoot](https://github.com/smicallef/spiderfoot) - Automated OSINT collection tool with over 200 data source modules.
- [Shodan](https://www.shodan.io) - Search engine for internet-connected devices and exposed services.
- [Censys](https://censys.io) - Attack surface search engine offering detailed host and certificate data.
- [Sherlock](https://github.com/sherlock-project/sherlock) - Hunts down social media accounts by username across many platforms.
- [holehe](https://github.com/megadose/holehe) - Checks whether an email address is registered on many websites.
- [GHunt](https://github.com/mxrch/GHunt) - Investigation tool for extracting information from Google accounts.
- [OSINT Framework](https://osintframework.com) - Web directory that organizes OSINT resources by category.
- [dnstwist](https://github.com/elceef/dnstwist) - Detects typosquatting, phishing, and brand impersonation via domain permutations.

## CTF Practice Platforms

- [Hack The Box](https://www.hackthebox.com) - Online lab of vulnerable machines and challenges across many skill areas.
- [TryHackMe](https://tryhackme.com) - Guided, beginner-friendly rooms and learning paths for offensive and defensive skills.
- [picoCTF](https://picoctf.org) - Free, permanent CTF and learning platform run by Carnegie Mellon University.
- [OverTheWire](https://overthewire.org/wargames/) - Classic wargames that teach security concepts through progressive Linux challenges.
- [Root-Me](https://www.root-me.org) - Large catalog of hacking challenges spanning web, network, forensics, and crypto.
- [PortSwigger Web Security Academy](https://portswigger.net/web-security) - Free, hands-on web security training with interactive labs.
- [pwn.college](https://pwn.college) - Free education platform from Arizona State University focused on binary exploitation.
- [CTFtime](https://ctftime.org) - Calendar, team rankings, and write-up archive for competitive CTF events.
- [HackThisSite](https://www.hackthissite.org) - Long-running free training ground with realistic security missions.

## Vulnerable Apps for Practice

- [DVWA](https://github.com/digininja/DVWA) - Damn Vulnerable Web Application, a PHP/MySQL app for practicing web attacks.
- [Metasploitable 3](https://github.com/rapid7/metasploitable3) - Purposely vulnerable Windows and Linux VM builds for exploitation practice.
- [Metasploitable 2](https://sourceforge.net/projects/metasploitable/) - Classic intentionally vulnerable Ubuntu VM widely used in tutorials.
- [OWASP Juice Shop](https://github.com/juice-shop/juice-shop) - Modern, feature-rich insecure web application covering the OWASP Top 10.
- [WebGoat](https://github.com/WebGoat/WebGoat) - Deliberately insecure Java application with guided lessons from OWASP.
- [Mutillidae II](https://github.com/webpwnized/mutillidae) - Free, open-source vulnerable web app with dozens of exploitable scenarios.
- [bWAPP](https://sourceforge.net/projects/bwapp/) - Buggy web application with over 100 web vulnerabilities to exploit.
- [VulnHub](https://www.vulnhub.com) - Repository of downloadable vulnerable VM images for offline practice.
- [Damn Vulnerable Web Services](https://github.com/snoopysecurity/dvws-node) - Insecure web app and API for learning web service and API testing.

## Certifications

- [OSCP (PEN-200)](https://www.offsec.com/courses/pen-200/) - Hands-on offensive security certification with a 24-hour practical exam.
- [OSEP (PEN-300)](https://www.offsec.com/courses/pen-300/) - Advanced OffSec course on evasion techniques and breaching mature environments.
- [CompTIA Security+](https://www.comptia.org/certifications/security) - Vendor-neutral entry-level certification covering core security concepts.
- [CompTIA PenTest+](https://www.comptia.org/certifications/pentest) - Intermediate certification focused on penetration testing and vulnerability management.
- [CEH](https://www.eccouncil.org/programs/certified-ethical-hacker-ceh/) - EC-Council certification covering a broad survey of hacking tools and techniques.
- [eJPT](https://security.ine.com/certifications/ejpt-certification/) - INE's beginner-level practical penetration testing certification.
- [GIAC GCIH](https://www.giac.org/certifications/certified-incident-handler-gcih/) - Incident handling and hacker exploit certification aimed at blue teams.
- [CRTP](https://www.alteredsecurity.com/adlab) - Altered Security's certification focused on Active Directory attack paths.
- [Blue Team Level 1 (BTL1)](https://securityblue.team/why-btl1/) - Practical defensive certification covering SOC analysis and incident response.
- [CISSP](https://www.isc2.org/certifications/cissp) - ISC2 management-level certification covering security governance and architecture.

## Cheat Sheets

- [PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings) - Massive collection of payloads and bypass techniques for web and network attacks.
- [HackTricks](https://book.hacktricks.xyz) - Community wiki of pentest tricks and methodology for nearly every attack surface.
- [GTFOBins](https://gtfobins.github.io) - Curated list of Unix binaries that can be abused to bypass local restrictions.
- [LOLBAS](https://lolbas-project.github.io) - Living Off The Land Binaries, Scripts and Libraries for Windows abuse.
- [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org) - Concise, high-value guidance on application security topics.
- [PentestMonkey Reverse Shell Cheat Sheet](https://pentestmonkey.net/cheat-sheet/shells/reverse-shell-cheat-sheet) - Reference one-liners for spawning reverse shells in many languages.
- [RevShells](https://www.revshells.com) - Interactive generator for reverse shell, bind shell, and MSFVenom payloads.
- [SANS Posters & Cheat Sheets](https://www.sans.org/posters/) - Free downloadable reference posters for blue team, DFIR, and cloud security.
- [explainshell](https://explainshell.com) - Breaks down any shell command and explains each flag from the man pages.

## Blogs & Newsletters

- [Krebs on Security](https://krebsonsecurity.com) - In-depth investigative reporting on cybercrime and the security industry.
- [Schneier on Security](https://www.schneier.com) - Bruce Schneier's long-running blog on cryptography, policy, and security thinking.
- [The Hacker News](https://thehackernews.com) - High-volume news site covering breaches, malware, and vulnerabilities.
- [BleepingComputer](https://www.bleepingcomputer.com) - News and technical write-ups on malware, ransomware, and incident response.
- [SANS Internet Storm Center](https://isc.sans.edu) - Daily diaries and analysis of current threats from volunteer handlers.
- [tl;dr sec](https://tldrsec.com) - Weekly newsletter summarizing the best AppSec and security research.
- [Google Project Zero](https://googleprojectzero.blogspot.com) - Deep technical write-ups of zero-day vulnerability research.
- [PortSwigger Research](https://portswigger.net/research) - Original web security research from the team behind Burp Suite.
- [Risky Business](https://risky.biz) - News podcast and newsletter covering security policy and industry trends.

## YouTube Channels & Podcasts

- [IppSec](https://www.youtube.com/@ippsec) - Detailed video walkthroughs of retired Hack The Box machines.
- [John Hammond](https://www.youtube.com/@_JohnHammond) - Malware analysis, CTF solves, and practical offensive security tutorials.
- [The Cyber Mentor](https://www.youtube.com/@TCMSecurityAcademy) - Practical ethical hacking courses and career advice.
- [LiveOverflow](https://www.youtube.com/@LiveOverflow) - Binary exploitation, reverse engineering, and security research explainers.
- [NetworkChuck](https://www.youtube.com/@NetworkChuck) - Approachable networking and security tutorials for newcomers.
- [Darknet Diaries](https://darknetdiaries.com) - Narrative podcast on true stories from the dark side of the internet.
- [Malicious Life](https://malicious.life) - Podcast on the history of cybersecurity, hackers, and major incidents.
- [Security Now](https://twit.tv/shows/security-now) - Weekly deep dive into security news and concepts with Steve Gibson.
- [SANS Blueprint Podcast](https://www.sans.org/podcasts/blueprint/) - Interviews focused on blue team tooling, detection, and defense.

## Books

- [Penetration Testing: A Hands-On Introduction to Hacking](https://nostarch.com/pentesting) - Georgia Weidman's practical primer covering the full assessment lifecycle.
- [The Hacker Playbook 3](https://securepla.net/hacker-playbook/) - Peter Kim's red team playbook structured around real engagement phases.
- [Black Hat Python, 2nd Edition](https://nostarch.com/black-hat-python2E) - Building offensive tooling and network hacks with Python.
- [The Web Application Hacker's Handbook](https://portswigger.net/web-security/web-application-hackers-handbook) - Foundational reference on finding and exploiting web application flaws.
- [The Practice of Network Security Monitoring](https://nostarch.com/nsm) - Richard Bejtlich on building detection and response around network data.
- [Practical Malware Analysis](https://nostarch.com/malware) - Hands-on guide to dissecting malicious software safely.
- [Nmap Network Scanning](https://nmap.org/book/) - The official Nmap reference guide, written by its author.
- [Network Security Assessment, 3rd Edition](https://www.oreilly.com/library/view/network-security-assessment/9781491910955/) - Chris McNab's methodology for testing networks and infrastructure.
- [Blue Team Handbook: Incident Response Edition](https://www.blueteamhandbook.com/) - Condensed field reference for incident responders and SOC analysts.

## Contributing

Contributions are very welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request, or use the [resource suggestion issue template](.github/ISSUE_TEMPLATE/resource-suggestion.md) if you would rather propose a resource without editing files yourself.

This list is released under [CC0 1.0 Universal](LICENSE) — to the extent possible under law, all copyright and related rights are waived.
