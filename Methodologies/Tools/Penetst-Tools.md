# Bug Bounty Checklist

## 1. Reconnaissance Techniques

### 1.1 Information Gathering<br />

- **Google Dorking :&emsp;** Use advanced search operators to find sensitive information.
    - ***Tools &emsp; =>*** &emsp; [Google Search](#) &emsp;|&emsp; [Shodan](#) &emsp;|&emsp; [Censys](#) &emsp;|&emsp; [Bing Search](#) &emsp;|&emsp; [DuckDuckGo](#) &emsp;|&emsp; [Google](https://www.google.com/) &emsp;|&emsp; [Google Advanced Search](https://www.google.com/advanced_search) &emsp;|&emsp;  [Google Search Guide](http://www.googleguide.com/print/adv_op_ref.pdf)<br />

- **WHOIS Lookup :&emsp;** Gather domain registration details.
    - ***Tools &emsp; =>*** &emsp; [WHOIS](#) &emsp;|&emsp;  [Domaintools](#) &emsp;|&emsp;  [WhoisXML API](#) &emsp;|&emsp;  [ARIN WHOIS](#) &emsp;|&emsp;  [RIPE NCC](#) &emsp;|&emsp;  [Domain Dossier](https://centralops.net/co/) &emsp;|&emsp;  [Whois Lookup](https://www.whois.com/)<br />

- **Reverse WHOIS Lookup :&emsp;** Find domains associated with a specific registrant.
    - ***Tools &emsp; =>*** &emsp; [WhoisXML API](#) &emsp;|&emsp;  [DomainTools](#) &emsp;|&emsp;  [ReverseWHOIS](#) &emsp;|&emsp;  [Robtex](#) &emsp;|&emsp;  [SecurityTrails](#) &emsp;|&emsp;  [Reverse WHOIS Lookup](https://whois.domaintools.com/)<br />

- **DNS Enumeration :&emsp;** Identify DNS records like A &emsp;|&emsp;  MX &emsp;|&emsp;  NS &emsp;|&emsp;  TXT &emsp;|&emsp;  SOA.
    - ***Tools &emsp; =>*** &emsp; [dnsenum](#) &emsp;|&emsp;  [dnsrecon](#) &emsp;|&emsp;  [dnspython](#) &emsp;|&emsp;  [dnsutils](#) &emsp;|&emsp;  [fierce](#) &emsp;|&emsp;  [dnsmap](#) &emsp;|&emsp;  [dnsx](#) &emsp;|&emsp;  [sublist3r](#) &emsp;|&emsp;  [theHarvester](#) &emsp;|&emsp;  [crt.sh](#) &emsp;|&emsp;  [DNSlytics](https://dnslytics.com/reverse-ip) &emsp;|&emsp;  [Pentest-Tools Subdomain Finder](https://pentest-tools.com/information-gathering/find-subdomains-of-domain#) &emsp;|&emsp;  [Spyse](https://spyse.com/) &emsp;|&emsp;  [Amass](https://github.com/OWASP/Amass) &emsp;|&emsp;  [Subfinder](https://github.com/projectdiscovery/subfinder) &emsp;|&emsp;  [Assetfinder](https://github.com/tomnomnom/assetfinder) &emsp;|&emsp;  [httprobe](https://github.com/tomnomnom/httprobe)<br />

- **IP Geolocation :&emsp;** Find the geographical location of IP addresses.
    - ***Tools &emsp; =>*** &emsp; [ipinfo](#) &emsp;|&emsp;  [ipapi](#) &emsp;|&emsp;  [geoip](#) &emsp;|&emsp;  [maxmind](#) &emsp;|&emsp;  [ipstack](#) &emsp;|&emsp;  [IPLocation.net](#) &emsp;|&emsp;  [ipgeolocation.io](#) &emsp;|&emsp;  [GeoIP2](#) &emsp;|&emsp;  [IPinfo](#) &emsp;|&emsp;  [DB-IP](#) &emsp;|&emsp;  [GeoGuessr](https://www.geoguessr.com) &emsp;|&emsp;  [GeoGuessr - The Top Tips &emsp;|&emsp;  Tricks and Techniques](https://somerandomstuff1.wordpress.com/2019/02/08/geoguessr-the-top-tips-tricks-and-techniques/)<br />

- **Public Records Search :&emsp;** Access public records related to the target.
    - ***Tools &emsp; =>*** &emsp; [Pipl](#) &emsp;|&emsp;  [Spokeo](#) &emsp;|&emsp;  [PeopleFinder](#) &emsp;|&emsp;  [Intelius](#) &emsp;|&emsp;  [LinkedIn](#) &emsp;|&emsp;  [Facebook](#) &emsp;|&emsp;  [Whitepages](#) &emsp;|&emsp;  [PublicRecords.com](#) &emsp;|&emsp;  [ZabaSearch](#) &emsp;|&emsp;  [BeenVerified](#) &emsp;|&emsp;  [WhitePages](https://www.whitepages.com/) &emsp;|&emsp;  [TruePeopleSearch](https://www.truepeoplesearch.com/) &emsp;|&emsp;  [FastPeopleSearch](https://www.fastpeoplesearch.com/) &emsp;|&emsp;  [FastBackgroundCheck](https://www.fastbackgroundcheck.com/) &emsp;|&emsp;  [411](https://www.411.com/) &emsp;|&emsp;  [Spokeo](https://www.spokeo.com/) &emsp;|&emsp;  [That'sThem](https://thatsthem.com/) &emsp;|&emsp;  [Voter Records](https://www.voterrecords.com)<br />

- **Search Engine Queries :&emsp;** Use search engines to gather information.
    - ***Tools &emsp; =>*** &emsp; [Google](#) &emsp;|&emsp;  [Bing](#) &emsp;|&emsp;  [DuckDuckGo](#) &emsp;|&emsp;  [Yandex](#) &emsp;|&emsp;  [Startpage](#) &emsp;|&emsp;  [Searx](#) &emsp;|&emsp;  [Blekko](#) &emsp;|&emsp;  [Qwant](#) &emsp;|&emsp;  [MetaCrawler](#) &emsp;|&emsp;  [WebCrawler](#) &emsp;|&emsp;  [Bing](https://www.bing.com/) &emsp;|&emsp;  [Bing Search Guide](https://www.bruceclay.com/blog/bing-google-advanced-search-operators/) &emsp;|&emsp;  [DuckDuckGo](https://duckduckgo.com/) &emsp;|&emsp;  [DuckDuckGo Search Guide](https://help.duckduckgo.com/duckduckgo-help-pages/results/syntax/) &emsp;|&emsp;  [Yandex](https://yandex.com/) &emsp;|&emsp;  [Baidu](http://www.baidu.com/)<br />

- **Breach Data Search :&emsp;** Check for data breaches with services like Have I Been Pwned.
    - ***Tools &emsp; =>*** &emsp; [Have I Been Pwned](#) &emsp;|&emsp;  [BreachDirectory](#) &emsp;|&emsp;  [DeHashed](#) &emsp;|&emsp;  [Leaks.ovh](#) &emsp;|&emsp;  [SpyCloud](#) &emsp;|&emsp;  [Pwned Passwords](#) &emsp;|&emsp;  [BreachAlarm](#) &emsp;|&emsp;  [Hacked Emails](#) &emsp;|&emsp;  [HackNotice](#) &emsp;|&emsp;  [BreachAuth](#) &emsp;|&emsp;  [Dehashed](https://dehashed.com/) &emsp;|&emsp;  [WeLeakInfo](https://weleakinfo.to/v2/) &emsp;|&emsp;  [LeakCheck](https://leakcheck.io/) &emsp;|&emsp;  [SnusBase](https://snusbase.com/) &emsp;|&emsp;  [Scylla.sh](https://scylla.sh/) &emsp;|&emsp;  [HaveIBeenPwned](https://haveibeenpwned.com/)<br />

- **Social Engineering Techniques :&emsp;** Use social tactics to gather information.
    - ***Tools &emsp; =>*** &emsp; [Social Engineering Toolkit](#) &emsp;|&emsp;  [Recon-ng](#) &emsp;|&emsp;  [Maltego](#) &emsp;|&emsp;  [OSINT Framework](#) &emsp;|&emsp;  [Hunter.io](#) &emsp;|&emsp;  [Email Hunter](#) &emsp;|&emsp;  [EmailPermutator](#) &emsp;|&emsp;  [LinkedIn](#) &emsp;|&emsp;  [Facebook](#) &emsp;|&emsp;  [Twitter](#) &emsp;|&emsp;  [Creating an Effective Sock Puppet for OSINT Investigations – Introduction](https://web.archive.org/web/20210125191016/https://jakecreps.com/2018/11/02/sock-puppets/) &emsp;|&emsp;  [The Art Of The Sock](https://www.secjuice.com/the-art-of-the-sock-osint-humint/) &emsp;|&emsp;  [Reddit - My process for setting up anonymous sockpuppet accounts](https://www.reddit.com/r/OSINT/comments/dp70jr/my_process_for_setting_up_anonymous_sockpuppet/)<br />

- **Publicly Available APIs :&emsp;** Analyze APIs for exposed information.
    - ***Tools &emsp; =>*** &emsp; [Postman](#) &emsp;|&emsp;  [Insomnia](#) &emsp;|&emsp;  [Swagger](#) &emsp;|&emsp;  [APIsec](#) &emsp;|&emsp;  [RapidAPI](#) &emsp;|&emsp;  [Shodan API](#) &emsp;|&emsp;  [Censys API](#) &emsp;|&emsp;  [Google Maps API](#) &emsp;|&emsp;  [IPinfo API](#) &emsp;|&emsp;  [VirusTotal API](#) &emsp;|&emsp;  [Clearbit Connect](https://chrome.google.com/webstore/detail/clearbit-connect-supercha/pmnhcgfcafcnkbengdcanjablaabjplo?hl=en)<br />

- **Certificate Transparency Logs :&emsp;** Monitor public logs for SSL certificates.
    - ***Tools &emsp; =>*** &emsp; [crt.sh](https://crt.sh/) &emsp;|&emsp;  [CertSpotter](#) &emsp;|&emsp;  [Google Certificate Transparency](#) &emsp;|&emsp;  [SSL Labs](#) &emsp;|&emsp;  [PassiveTotal](#) &emsp;|&emsp;  [CertStream](#) &emsp;|&emsp;  [Certificate Transparency Logs](#) &emsp;|&emsp;  [Symantec CT](#) &emsp;|&emsp;  [Cloudflare CT Logs](#) &emsp;|&emsp;  [HackerOne CT Logs](#)<br />

- **Domain History Analysis :&emsp;** Use tools to analyze historical domain data.
    - ***Tools &emsp; =>*** &emsp; [DomainTools](#), &emsp;|&emsp;  [WhoisXML API](#) &emsp;|&emsp;  [Wayback Machine](#) &emsp;|&emsp;  [Archive.org](#) &emsp;|&emsp;  [DNS History](#) &emsp;|&emsp;  [Historical WHOIS](#) &emsp;|&emsp;  [Netcraft](#) &emsp;|&emsp;  [Robtex](#) &emsp;|&emsp;  [SecurityTrails](#) &emsp;|&emsp;  [BuiltWith](#) &emsp;|&emsp;  [BuiltWith](https://builtwith.com/) &emsp;|&emsp;  [View DNS](https://viewdns.info/)<br />

### 1.2 Subdomain and Domain Discovery<br />

- **Subdomain Enumeration :&emsp;** Discover subdomains using tools like Sublist3r or Amass.
    - ***Tools &emsp; =>*** &emsp; [Sublist3r](#) &emsp;|&emsp;  [Amass](#), &emsp;|&emsp;  [Subfinder](#) &emsp;|&emsp;  [Findomain](#) &emsp;|&emsp;  [Subjack](#) &emsp;|&emsp;  [Assetfinder](#) &emsp;|&emsp;  [Knockpy](#) &emsp;|&emsp;  [Subzy](#) &emsp;|&emsp;  [Subdomainizer](#) &emsp;|&emsp;  [CRT.sh](#) &emsp;|&emsp;  [Pentest-Tools Subdomain Finder](https://pentest-tools.com/information-gathering/find-subdomains-of-domain#) &emsp;|&emsp;  [Subfinder](https://github.com/projectdiscovery/subfinder) &emsp;|&emsp;  [Assetfinder](https://github.com/tomnomnom/assetfinder)<br />

- **Reverse IP Lookup :&emsp;** Identify other domains hosted on the same IP.
    - ***Tools &emsp; =>*** &emsp; [Reverse IP Lookup](#) &emsp;|&emsp;  [Robtex](#) &emsp;|&emsp;  [SecurityTrails](#) &emsp;|&emsp;  [Shodan](#) &emsp;|&emsp;  [Censys](#) &emsp;|&emsp;  [Netcraft](#) &emsp;|&emsp;  [DNSdumpster](#) &emsp;|&emsp;  [Spyse](#) &emsp;|&emsp;  [ThreatMiner](#) &emsp;|&emsp;  [Webscan](#) &emsp;|&emsp;  [DNSlytics](https://dnslytics.com/reverse-ip) &emsp;|&emsp;  [View DNS](https://viewdns.info/)<br />

- **DNS Dumpster Diving :&emsp;** Extract information about DNS records.
    - ***Tools &emsp; =>*** &emsp; [dnsdumpster](#) &emsp;|&emsp;  [dnsrecon](#) &emsp;|&emsp;  [dnstracer](#) &emsp;|&emsp;  [dnsutils](#) &emsp;|&emsp;  [DNSMap](#) &emsp;|&emsp;  [Fierce](#) &emsp;|&emsp;  [Netcraft](#) &emsp;|&emsp;  [Google DNS](#) &emsp;|&emsp;  [SecurityTrails](#) &emsp;|&emsp;  [Shodan](#) &emsp;|&emsp;  [DNSDumpster](https://dnsdumpster.com/)<br />

- **Zone Transfers :&emsp;** Attempt DNS zone transfers to gather records.
    - ***Tools &emsp; =>*** &emsp; [dig](#) &emsp;|&emsp;  [nslookup](#) &emsp;|&emsp;  [dnsrecon](#) &emsp;|&emsp;  [Fierce](#) &emsp;|&emsp;  [DNSMap](#) &emsp;|&emsp;  [dnstracer](#) &emsp;|&emsp;  [dnsscan](#) &emsp;|&emsp;  [Zone Transfer Scanner](#) &emsp;|&emsp;  [Recon-ng](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [Zone Transfer](https://www.zone-transfer.com/) <br />

### 1.3 Technology and Service Identification<br />

- **Website Footprinting :&emsp;** Identify technologies &emsp;|&emsp;  server details &emsp;|&emsp;  and software versions.
    - ***Tools &emsp; =>*** &emsp; [Wappalyzer](#) &emsp;|&emsp;  [WhatWeb](#) &emsp;|&emsp;  [Shodan](#) &emsp;|&emsp;  [Censys](#) &emsp;|&emsp;  [HTTP Headers](#) &emsp;|&emsp;  [Wappalyzer](#) &emsp;|&emsp;  [WhatCMS](#) &emsp;|&emsp;  [Gau](#) &emsp;|&emsp;  [BuiltWith](https://builtwith.com/) &emsp;|&emsp;  [Netcraft Site Reports](https://sitelogs.netcraft.com/)<br />

- **Shodan Search :&emsp;** Find internet-connected devices and their details.
    - ***Tools &emsp; =>*** &emsp; [Shodan](https://shodan.io) &emsp;|&emsp;  [Censys](#) &emsp;|&emsp;  [ZoomEye](#) &emsp;|&emsp;  [BinaryEdge](#) &emsp;|&emsp;  [Fofa](#) &emsp;|&emsp;  [Rapid7](#) &emsp;|&emsp;  [GreyNoise](#) &emsp;|&emsp;  [Pulsedive](#) &emsp;|&emsp;  [ThreatQuotient](#) &emsp;|&emsp;  [RATelnet](#)<br />

- **Censys Search :&emsp;** Identify and analyze devices and systems.
    - ***Tools &emsp; =>*** &emsp; [Censys](https://censys.io/) &emsp;|&emsp;  [Shodan](#) &emsp;|&emsp;  [ZoomEye](#) &emsp;|&emsp;  [BinaryEdge](#) &emsp;|&emsp;  [Fofa](#) &emsp;|&emsp;  [Rapid7](#) &emsp;|&emsp;  [GreyNoise](#) &emsp;|&emsp;  [Pulsedive](#) &emsp;|&emsp;  [ThreatQuotient](#) &emsp;|&emsp;  [RATelnet](#)<br />

- **SSL/TLS Certificate Analysis :&emsp;** Review certificates for associated domains.
    - ***Tools &emsp; =>*** &emsp; [testssl](https://github.com/drwetter/testssl.sh) &emsp;|&emsp;  [SSL Labs](https://www.ssllabs.com/ssltest/) &emsp;|&emsp;  [CertSpotter](#) &emsp;|&emsp;  [crt.sh](#) &emsp;|&emsp;  [SSL Certificate Checker](#) &emsp;|&emsp;  [Shodan](#) &emsp;|&emsp;  [Censys](#) &emsp;|&emsp;  [SecurityTrails](#) &emsp;|&emsp;  [SSL Labs](#) &emsp;|&emsp;  [CertStream](#) &emsp;|&emsp;  [SSL Checker](#)<br />

- **Web Application Framework Identification :&emsp;** Determine the frameworks used on a website.
    - ***Tools &emsp; =>*** &emsp; [Wappalyzer](#) &emsp;|&emsp;  [WhatWeb](#) &emsp;|&emsp;  [BuiltWith](#) &emsp;|&emsp;  [Netcraft](#) &emsp;|&emsp;  [CMS Detector](#) &emsp;|&emsp;  [Framework Scanner](#) &emsp;|&emsp;  [HTTP Headers](#) &emsp;|&emsp;  [Wappalyzer](#) &emsp;|&emsp;  [WebTech](#) &emsp;|&emsp;  [AppDetective](#) &emsp;|&emsp;  [BuiltWith](https://builtwith.com/)<br />

- **Netcraft Site Reports :&emsp;** Analyze site reports for server details and technologies.
    - ***Tools &emsp; =>*** &emsp; [Netcraft](#) &emsp;|&emsp;  [BuiltWith](#) &emsp;|&emsp;  [Wappalyzer](#) &emsp;|&emsp;  [WhatWeb](#) &emsp;|&emsp;  [Shodan](#) &emsp;|&emsp;  [Censys](#) &emsp;|&emsp;  [SecurityTrails](#) &emsp;|&emsp;  [SSL Labs](#) &emsp;|&emsp;  [Wayback Machine](#) &emsp;|&emsp;  [Webscreenshot](#)

### 1.4 Metadata and Historical Data<br />

- **FOCA :&emsp;** Extract metadata from documents and images.
    - ***Tools &emsp; =>*** &emsp; [FOCA](https://www.elevenpaths.com/labs/foca/index.html) &emsp;|&emsp;  [ExifTool](#) &emsp;|&emsp;  [Metadata Extractor](#) &emsp;|&emsp;  [ExifPilot](#) &emsp;|&emsp;  [Metagoofil](#) &emsp;|&emsp;  [DocScraper](#) &emsp;|&emsp;  [PDF-Analyzer](#) &emsp;|&emsp;  [X1](#) &emsp;|&emsp;  [Metagoofil](#) &emsp;|&emsp;  [ExifTool](#)<br />

- **ExifTool :&emsp;** Extract metadata from files and images.
    - ***Tools &emsp; =>*** &emsp; [Jeffrey's Image Metadata Viewer](http://exif.regex.info/exif.cgi) &emsp;|&emsp;  [ExifTool](#) &emsp;|&emsp;  [FOCA](#) &emsp;|&emsp;  [Metadata Extractor](#) &emsp;|&emsp;  [ExifPilot](#) &emsp;|&emsp;  [DocScraper](#) &emsp;|&emsp;  [PDF-Analyzer](#) &emsp;|&emsp;  [X1](#) &emsp;|&emsp;  [Metagoofil](#) &emsp;|&emsp;  [ExifTool](#) &emsp;|&emsp;  [Metadata++](#)<br />

- **Wayback Machine :&emsp;** Retrieve historical versions of web pages.
    - ***Tools &emsp; =>*** &emsp; [Wayback Machine](https://web.archive.org/) &emsp;|&emsp;  [Archive.org](#) &emsp;|&emsp;  [Oldweb.today](#) &emsp;|&emsp;  [WebCite](#) &emsp;|&emsp;  [PageFreezer](#) &emsp;|&emsp;  [Google Cache](#) &emsp;|&emsp;  [Bing Cache](#) &emsp;|&emsp;  [Yandex Cache](#) &emsp;|&emsp;  [Wayback Machine API](#) &emsp;|&emsp;  [Netarchive](#)<br />

- **Github Repository Search :&emsp;** Look for sensitive information in code repositories.
    - ***Tools &emsp; =>*** &emsp; [Github](https://github.com/) &emsp;|&emsp;  [GitHub Code Search](#) &emsp;|&emsp;  [GitHound](#) &emsp;|&emsp;  [TruffleHog](#) &emsp;|&emsp;  [Repo-Extractor](#) &emsp;|&emsp;  [GitSecrets](#) &emsp;|&emsp;  [Gitleaks](#) &emsp;|&emsp;  [GitRob](#) &emsp;|&emsp;  [GitGuardian](#) &emsp;|&emsp;  [GitGraber](#)<br />

- **Metadata Analysis :&emsp;** Analyze file and document metadata.
    - ***Tools &emsp; =>*** &emsp; [ExifTool](http://exif.regex.info/exif.cgi) &emsp;|&emsp;  [FOCA](#) &emsp;|&emsp;  [Metadata Extractor](#) &emsp;|&emsp;  [DocScraper](#) &emsp;|&emsp;  [PDF-Analyzer](#) &emsp;|&emsp;  [Metagoofil](#) &emsp;|&emsp;  [X1](#) &emsp;|&emsp;  [Metagoofil](#) &emsp;|&emsp;  [Metadata++](#)

### 1.5 Network and Traffic Analysis<br />

- **Network Mapping :&emsp;** Map out network topology with tools like Nmap.
    - ***Tools &emsp; =>*** &emsp; [Nmap](https://nmap.org/) &emsp;|&emsp;  [Masscan](#) &emsp;|&emsp;  [Zenmap](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [Angry IP Scanner](#) &emsp;|&emsp;  [Unicornscan](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [Advanced IP Scanner](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [Netdiscover](#)<br />

- **Network Traffic Analysis :&emsp;** Analyze network traffic for service and system information.
    - ***Tools &emsp; =>*** &emsp; [Wireshark](https://www.wireshark.org/) &emsp;|&emsp;  [tcpdump](#) &emsp;|&emsp;  [Tshark](#) &emsp;|&emsp;  [Kismet](#) &emsp;|&emsp;  [NetworkMiner](#) &emsp;|&emsp;  [Zeek](#) &emsp;|&emsp;  [EtherApe](#) &emsp;|&emsp;  [Snort](#) &emsp;|&emsp;  [NetFlow](#) &emsp;|&emsp;  [Colasoft Capsa](#)<br />

- **IP Range Scanning :&emsp;** Identify IP ranges associated with the target.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [Masscan](#) &emsp;|&emsp;  [Zmap](#) &emsp;|&emsp;  [Unicornscan](#) &emsp;|&emsp;  [Netdiscover](#) &emsp;|&emsp;  [Angry IP Scanner](#) &emsp;|&emsp;  [Advanced IP Scanner](#) &emsp;|&emsp;  [Fping](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [Shodan](#)<br />

- **Network Enumeration :&emsp;** Use traceroute to identify network paths.
    - ***Tools &emsp; =>*** &emsp; [Traceroute](#) &emsp;|&emsp;  [MTR](#) &emsp;|&emsp;  [PingPlotter](#) &emsp;|&emsp;  [PathPing](#) &emsp;|&emsp;  [Tracert](#) &emsp;|&emsp;  [NetworkMiner](#) &emsp;|&emsp;  [TraceRoute](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Hping](#) &emsp;|&emsp;  [OpenVAS](#)

## 2. Enumeration Techniques

### 2.1 Service and Port Enumeration<br />

- **Service Enumeration :&emsp;** Identify active services and their versions.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [Masscan](#) &emsp;|&emsp;  [Service Scanner](#) &emsp;|&emsp;  [Zmap](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [Shodan](#) &emsp;|&emsp;  [Censys](#) &emsp;|&emsp;  [TCP Port Scanner](#)<br />

- **Port Scanning :&emsp;** Identify open ports and services running on the target.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [Masscan](#) &emsp;|&emsp;  [Zmap](#) &emsp;|&emsp;  [Unicornscan](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [Angry IP Scanner](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [PortQry](#) &emsp;|&emsp;  [Fping](#)<br />

- **Banner Grabbing :&emsp;** Obtain service banners to determine versions.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [Telnet](#) &emsp;|&emsp;  [BannerGrab](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [Telnet](#) &emsp;|&emsp;  [WhatWeb](#) &emsp;|&emsp;  [Shodan](#) &emsp;|&emsp;  [Censys](#) &emsp;|&emsp;  [BannerGrabber](#)<br />

- **FTP Enumeration :&emsp;** List files and directories on FTP servers.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [ftp](#) &emsp;|&emsp;  [NcFTP](#) &emsp;|&emsp;  [WinSCP](#) &emsp;|&emsp;  [FileZilla](#) &emsp;|&emsp;  [FTPScan](#) &emsp;|&emsp;  [Hydra](#) &emsp;|&emsp;  [FTPEnum](#) &emsp;|&emsp;  [Burp Suite](#)<br />

- **HTTP Methods Testing :&emsp;** Check for supported HTTP methods.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [Burp Suite](#) &emsp;|&emsp;  [OWASP ZAP](#) &emsp;|&emsp;  [Nikto](#) &emsp;|&emsp;  [HTTP Methods](#) &emsp;|&emsp;  [Wapiti](#) &emsp;|&emsp;  [WhatWeb](#) &emsp;|&emsp;  [Dirb](#) &emsp;|&emsp;  [Gau](#) &emsp;|&emsp;  [HTTPX](#)<br />

- **WebDAV Enumeration :&emsp;** Explore WebDAV services for vulnerabilities.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [Burp Suite](#) &emsp;|&emsp;  [OWASP ZAP](#) &emsp;|&emsp;  [Nikto](#) &emsp;|&emsp;  [WebDAV Scanner](#) &emsp;|&emsp;  [dirb](#) &emsp;|&emsp;  [Wapiti](#) &emsp;|&emsp;  [Gau](#) &emsp;|&emsp;  [HTTPX](#) &emsp;|&emsp;  [WebDAV](#)<br />

- **NFS Enumeration :&emsp;** Identify Network File System shares and permissions.
    - ***Tools &emsp; =>*** &emsp; [showmount](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [rpcinfo](#) &emsp;|&emsp;  [nfsstat](#) &emsp;|&emsp;  [nmap -p 2049](#) &emsp;|&emsp;  [nfs-common](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [Hydra](#)

### 2.2 User and Resource Enumeration<br />

- **User Enumeration :&emsp;** Find valid usernames using tools like Hydra or Medusa.
    - ***Tools &emsp; =>*** &emsp; [Enum4linux](https://github.com/portcullislabs/enum4linux) &emsp;|&emsp;  [Hydra](#) &emsp;|&emsp;  [Medusa](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [Snmpwalk](#) &emsp;|&emsp;  [SMBclient](#) &emsp;|&emsp;  [LDAP Enumeration](#) &emsp;|&emsp;  [Kerberos Enumeration](#) &emsp;|&emsp;  [Fuzzdb](#)<br />

- **SMB Enumeration :&emsp;** Extract information from SMB shares using tools like enum4linux.
    - ***Tools &emsp; =>*** &emsp; [enum4linux](#) &emsp;|&emsp;  [SMBclient](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [SMBMap](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [SMBScanner](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [Impacket](#)<br />

- **NetBIOS Enumeration :&emsp;** Gather NetBIOS information with nbtstat.
    - ***Tools &emsp; =>*** &emsp; [nbtscan](https://sourceforge.net/projects/nbtscan/) &emsp;|&emsp;  [nbtstat](#) &emsp;|&emsp;  [NetBIOS Scanner](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [SMBclient](#) &emsp;|&emsp;  [NetView](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [Hydra](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [Smbclient](#)<br />

- **SNMP Enumeration :&emsp;** Extract SNMP data with snmpwalk.
    - ***Tools &emsp; =>*** &emsp; [snmpwalk](https://linux.die.net/man/1/snmpwalk) &emsp;|&emsp;  [snmpwalk](#) &emsp;|&emsp;  [nmap](#) &emsp;|&emsp;  [onesixtyone](#) &emsp;|&emsp;  [snmpenum](#) &emsp;|&emsp;  [snmpcheck](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [SolarWinds](#) &emsp;|&emsp;  [SolarWinds SNMP Walk](#)<br />

- **LDAP Enumeration :&emsp;** Query LDAP servers for user and group details.
    - ***Tools &emsp; =>*** &emsp; [ldapsearch](https://linux.die.net/man/1/ldapsearch) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [LDAP Enumeration](#) &emsp;|&emsp;  [LDAPScan](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [Ldapdomaindump](#)<br />

- **SMTP Enumeration :&emsp;** Discover email configurations using tools like SMTPSend.
    - ***Tools &emsp; =>*** &emsp; [SMTP Enumerator](https://github.com/OsandaMalith/SMTP-Enumerator) &emsp;|&emsp;  [smtp-user-enum](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [SMTPSend](#) &emsp;|&emsp;  [SMTPScan](#) &emsp;|&emsp;  [SMTP Enumeration](#) &emsp;|&emsp;  [Harvester](#) &emsp;|&emsp;  [Snmpwalk](#) &emsp;|&emsp;  [Burp Suite](#) &emsp;|&emsp;  [EmailHunter](#)<br />

- **Kerberos Enumeration :&emsp;** Enumerate Kerberos tickets and services.
    - ***Tools &emsp; =>*** &emsp; [Kerberoasting](https://www.sans.org/white-papers/34610/) &emsp;|&emsp;  [Kerberoast](#) &emsp;|&emsp;  [Rubeus](#) &emsp;|&emsp;  [Impacket](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [Evil-WinRM](#) &emsp;|&emsp;  [GetNPUsers](#) &emsp;|&emsp;  [PowerView](#) &emsp;|&emsp;  [BloodHound](#)<br />

- **RPC Enumeration :&emsp;** Identify RPC services and versions.
    - ***Tools &emsp; =>*** &emsp; [rpcclient](https://linux.die.net/man/1/rpcclient) &emsp;|&emsp;  [rpcinfo](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [SMBclient](#) &emsp;|&emsp;  [Hydra](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [RPCScan](#)<br />

- **LDAP Injection Testing :&emsp;** Test for LDAP injection vulnerabilities.
    - ***Tools &emsp; =>*** &emsp; [OWASP ZAP](https://owasp.org/www-project-zap/) &emsp;|&emsp;  [LDAPInjection](#) &emsp;|&emsp;  [Burp Suite](#) &emsp;|&emsp;  [OWASP ZAP](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [Sqlmap](#) &emsp;|&emsp;  [LDAPi](#) &emsp;|&emsp;  [Fuzzdb](#) &emsp;|&emsp;  [DirBuster](#) &emsp;|&emsp;  [Gf](#)<br />

- **Kerberoasting :&emsp;** Extract and crack service tickets from Kerberos.
    - ***Tools &emsp; =>*** &emsp; [Kerberoasting](https://www.sans.org/white-papers/34610/) &emsp;|&emsp;  [Rubeus](#) &emsp;|&emsp;  [Impacket](#) &emsp;|&emsp;  [Kerberoast](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [PowerView](#) &emsp;|&emsp;  [BloodHound](#) &emsp;|&emsp;  [GetNPUsers](#) &emsp;|&emsp;  [Kerbrute](#) &emsp;|&emsp;  [Kerbrute](#)

## 3. Scanning Techniques

### 3.1 Network and Service Scanning<br />

- **Network Scanning :&emsp;** Discover live hosts and network services.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [Masscan](#) &emsp;|&emsp;  [Zmap](#) &emsp;|&emsp;  [Unicornscan](#) &emsp;|&emsp;  [Netdiscover](#) &emsp;|&emsp;  [Angry IP Scanner](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [Advanced IP Scanner](#)<br />

- **Port Scanning :&emsp;** Identify open ports with detailed options.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [Masscan](#) &emsp;|&emsp;  [Zmap](#) &emsp;|&emsp;  [Unicornscan](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [Angry IP Scanner](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [PortQry](#) &emsp;|&emsp;  [Fping](#)<br />

- **Service Scanning :&emsp;** Determine services running on open ports.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [Masscan](#) &emsp;|&emsp;  [Zmap](#) &emsp;|&emsp;  [Unicornscan](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [Shodan](#) &emsp;|&emsp;  [Censys](#) &emsp;|&emsp;  [TCP Port Scanner](#)<br />

- **Operating System Fingerprinting :&emsp;** Identify the operating system using tools like Nmap or p0f.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [p0f](#) &emsp;|&emsp;  [Xprobe2](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [Shodan](#) &emsp;|&emsp;  [Censys](#) &emsp;|&emsp;  [OS Fingerprinter](#) &emsp;|&emsp;  [P0f](#) &emsp;|&emsp;  [Netcat](#)<br />

- **Web Application Scanning :&emsp;** Detect vulnerabilities in web applications using tools like OWASP ZAP or Burp Suite.
    - ***Tools &emsp; =>*** &emsp; [OWASP ZAP](#) &emsp;|&emsp;  [Burp Suite](#) &emsp;|&emsp;  [Nikto](#) &emsp;|&emsp;  [Wapiti](#) &emsp;|&emsp;  [Arachni](#) &emsp;|&emsp;  [Acunetix](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [W3af](#) &emsp;|&emsp;  [SQLMap](#)<br />

- **DNS Scanning :&emsp;** Scan DNS records and identify potential misconfigurations.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [dnsenum](#) &emsp;|&emsp;  [dnsrecon](#) &emsp;|&emsp;  [dnsutils](#) &emsp;|&emsp;  [dnsmap](#) &emsp;|&emsp;  [fierce](#) &emsp;|&emsp;  [DNSEnum](#) &emsp;|&emsp;  [DNSRecon](#) &emsp;|&emsp;  [DNSMap](#) &emsp;|&emsp;  [Fierce](#)<br />

- **SSL/TLS Scanning :&emsp;** Check SSL/TLS configurations and vulnerabilities using tools like Qualys SSL Labs.
    - ***Tools &emsp; =>*** &emsp; [testssl](https://github.com/drwetter/testssl.sh) &emsp;|&emsp;  [Qualys SSL Labs](#) &emsp;|&emsp;  [SSLLabs](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [OpenSSL](#) &emsp;|&emsp;  [SSLScan](#) &emsp;|&emsp;  [TestSSL](#) &emsp;|&emsp;  [SSLYze](#) &emsp;|&emsp;  [Cipherscan](#) &emsp;|&emsp;  [SSLStrip](#) &emsp;|&emsp;  [Hardenize](#)

### 3.2 Vulnerability and Protocol Scanning<br />

- **Vulnerability Scanning :&emsp;** Identify known vulnerabilities using tools like Nessus or OpenVAS.
    - ***Tools &emsp; =>*** &emsp; [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [Qualys](#) &emsp;|&emsp;  [Rapid7 InsightVM](#) &emsp;|&emsp;  [Burp Suite](#) &emsp;|&emsp;  [Acunetix](#) &emsp;|&emsp;  [Wapiti](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Arachni](#) &emsp;|&emsp;  [AppScan](#)<br />

- **Port Sweeping :&emsp;** Scan a range of ports to identify open services.
    - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp;  [Masscan](#) &emsp;|&emsp;  [Zmap](#) &emsp;|&emsp;  [Unicornscan](#) &emsp;|&emsp;  [Fping](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [Angry IP Scanner](#) &emsp;|&emsp;  [PortQry](#) &emsp;|&emsp;  [Zmap](#) &emsp;|&emsp;  [Netdiscover](#)<br />

- **Application Scanning :&emsp;** Identify vulnerabilities in applications and services.
    - ***Tools &emsp; =>*** &emsp; [OWASP ZAP](#) &emsp;|&emsp;  [Burp Suite](#) &emsp;|&emsp;  [Nessus](#) &emsp;|&emsp;  [OpenVAS](#) &emsp;|&emsp;  [Acunetix](#) &emsp;|&emsp;  [AppScan](#) &emsp;|&emsp;  [Wapiti](#) &emsp;|&emsp;  [Arachni](#) &emsp;|&emsp;  [AppSpider](#) &emsp;|&emsp;  [Nikto](#)<br />

- **Network Protocol Analysis :&emsp;** Analyze network protocols for weaknesses.
    - ***Tools &emsp; =>*** &emsp; [Wireshark](#) &emsp;|&emsp;  [tcpdump](#) &emsp;|&emsp;  [Tshark](#) &emsp;|&emsp;  [Kismet](#) &emsp;|&emsp;  [NetFlow](#) &emsp;|&emsp;  [Snort](#) &emsp;|&emsp;  [Zeek](#) &emsp;|&emsp;  [Colasoft Capsa](#) &emsp;|&emsp;  [NetworkMiner](#) &emsp;|&emsp;  [Suricata](#)<br />

- **Wireless Scanning :&emsp;** Identify and analyze wireless networks and their security settings.
    - ***Tools &emsp; =>*** &emsp; [Kismet](https://kismetwireless.net/) &emsp;|&emsp;  [Aircrack-ng](#) &emsp;|&emsp;  [Wireshark](#) &emsp;|&emsp;  [Reaver](#) &emsp;|&emsp;  [Fern Wifi Cracker](#) &emsp;|&emsp;  [Wifite](#) &emsp;|&emsp;  [NetStumbler](#) &emsp;|&emsp;  [InSSIDer](#) &emsp;|&emsp;  [Airodump-ng](#) &emsp;|&emsp;  [WPS Cracker](#)

## 4. OSINT Techniques
<br />

- **Social Media Analysis :&emsp;** Collect information from social media platforms.
    - ***Tools &emsp; =>*** &emsp; [Maltego](#) &emsp;|&emsp;  [Social-Engineer Toolkit](#) &emsp;|&emsp;  [Recon-ng](#) &emsp;|&emsp;  [Spokeo](#) &emsp;|&emsp;  [Pipl](#) &emsp;|&emsp;  [LinkedIn](#) &emsp;|&emsp;  [Facebook](#) &emsp;|&emsp;  [Twitter](#) &emsp;|&emsp;  [Instagram](#) &emsp;|&emsp;  [Social Mapper](#) &emsp;|&emsp;  [Social Bearing](https://socialbearing.com/) &emsp;|&emsp;  [Twitonomy](https://www.twitonomy.com/) &emsp;|&emsp;  [TweetDeck](https://tweetdeck.com/)<br />

- **Public Records Search :&emsp;** Access public records and databases.
    - ***Tools &emsp; =>*** &emsp; [Pipl](#) &emsp;|&emsp;  [Spokeo](#) &emsp;|&emsp;  [PeopleFinder](#) &emsp;|&emsp;  [Intelius](#) &emsp;|&emsp;  [LinkedIn](#) &emsp;|&emsp;  [Facebook](#) &emsp;|&emsp;  [Whitepages](#) &emsp;|&emsp;  [PublicRecords.com](#) &emsp;|&emsp;  [ZabaSearch](#) &emsp;|&emsp;  [BeenVerified](#)<br />

- **Domain and IP Lookup :&emsp;** Investigate domain and IP address information.
    - ***Tools &emsp; =>*** &emsp; [WHOIS](#) &emsp;|&emsp;  [DomainTools](#) &emsp;|&emsp;  [ipinfo](#) &emsp;|&emsp;  [Censys](#) &emsp;|&emsp;  [Shodan](#) &emsp;|&emsp;  [Google Search](#) &emsp;|&emsp;  [Bing Search](#) &emsp;|&emsp;  [dnsenum](#) &emsp;|&emsp;  [dnsrecon](#) 
[ipapi]&emsp;&emsp; <br />

- **Historical Data Search :&emsp;** Access historical data on websites and domains.
    - ***Tools &emsp; =>*** &emsp; [Wayback Machine](#) &emsp;|&emsp;  [Archive.org](#) &emsp;|&emsp;  [Oldweb.today](#) &emsp;|&emsp;  [WebCite](#) &emsp;|&emsp;  [PageFreezer](#) &emsp;|&emsp;  [Google Cache](#) &emsp;|&emsp;  [Bing Cache](#) &emsp;|&emsp;  [Yandex Cache](#) &emsp;|&emsp;  [Netarchive](#) &emsp;|&emsp;  [Wayback Machine API](#)<br />

- **Code Repository Search :&emsp;** Look for sensitive information in public code repositories.
    - ***Tools &emsp; =>*** &emsp; [Github Search](#) &emsp;|&emsp;  [GitHub Code Search](#) &emsp;|&emsp;  [GitHound](#) &emsp;|&emsp;  [TruffleHog](#) &emsp;|&emsp;  [Repo-Extractor](#) &emsp;|&emsp;  [GitSecrets](#) &emsp;|&emsp;  [Gitleaks](#) &emsp;|&emsp;  [GitRob](#) &emsp;|&emsp;  [GitGuardian](#) &emsp;|&emsp;  [GitGraber](#)<br />

- **Online People Search :&emsp;** Find personal details and professional backgrounds.
    - ***Tools &emsp; =>*** &emsp; [Pipl](#) &emsp;|&emsp;  [Intelius](#) &emsp;|&emsp;  [Spokeo](#) &emsp;|&emsp;  [PeopleFinders](#) &emsp;|&emsp;  [LinkedIn](#) &emsp;|&emsp;  [Facebook](#) &emsp;|&emsp;  [Whitepages](#) &emsp;|&emsp;  [BeenVerified](#) &emsp;|&emsp;  [ZabaSearch](#) &emsp;|&emsp;  [PublicRecords.com](#)<br />

- **Technical Analysis :&emsp;** Analyze publicly available technical data.
    - ***Tools &emsp; =>*** &emsp; [Shodan](#) &emsp;|&emsp;  [Censys](#) &emsp;|&emsp;  [Google Search](#) &emsp;|&emsp;  [Bing Search](#) &emsp;|&emsp;  [CVE Details](#) &emsp;|&emsp;  [Exploit-DB](#) &emsp;|&emsp;  [Mitre ATT&CK](#) &emsp;|&emsp;  [Common Vuln. Scoring System (CVSS)](#) &emsp;|&emsp;  [NVD](#) &emsp;|&emsp;  [OSINT Framework](#)

## 5. Active Directory Enumeration <br />

- **Domain Enumeration :&emsp;** Gather information about the domain structure.
    - ***Tools &emsp; =>*** &emsp; [AD Pentesters](https://github.com/0xDigimon/PenetrationTesting_Notes-) &emsp;|&emsp;  [BloodHound](#) &emsp;|&emsp;  [PowerView](#) &emsp;|&emsp;  [ADRecon](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [LDAP Enumeration](#) &emsp;|&emsp;  [Kerberos Enumeration](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [Impacket](#) &emsp;|&emsp;  [Pentest-Tools Subdomain Finder](https://pentest-tools.com/information-gathering/find-subdomains-of-domain#) &emsp;|&emsp;  [Subfinder](https://github.com/projectdiscovery/subfinder) &emsp;|&emsp;  [Assetfinder](https://github.com/tomnomnom/assetfinder)<br />

- **User Enumeration :&emsp;** Identify domain users.
    - ***Tools &emsp; =>*** &emsp; [BloodHound](#) &emsp;|&emsp;  [PowerView](#) &emsp;|&emsp;  [ADRecon](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Kerberos Enumeration](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [Impacket](#) &emsp;|&emsp;  [NetUser](#) &emsp;|&emsp;  [ADfind](#) &emsp;|&emsp;  [Enum4linux](https://github.com/portcullislabs/enum4linux)<br />

- **Group Enumeration :&emsp;** Discover groups and their memberships.
    - ***Tools &emsp; =>*** &emsp; [BloodHound](#) &emsp;|&emsp;  [PowerView](#) &emsp;|&emsp;  [ADRecon](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Kerberos Enumeration](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [Impacket](#) &emsp;|&emsp;  [NetGroup](#) &emsp;|&emsp;  [ADfind](#)<br />

- **Domain Trust Enumeration :&emsp;** Identify domain trusts and relationships.
    - ***Tools &emsp; =>*** &emsp; [BloodHound](#) &emsp;|&emsp;  [PowerView](#) &emsp;|&emsp;  [ADRecon](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Kerberos Enumeration](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [Impacket](#) &emsp;|&emsp;  [Netdom](#) &emsp;|&emsp;  [TrustInspector](#)<br />

- **ACL Enumeration :&emsp;** Review Access Control Lists for misconfigurations.
    - ***Tools &emsp; =>*** &emsp; [BloodHound](#) &emsp;|&emsp;  [PowerView](#) &emsp;|&emsp;  [ADRecon](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Kerberos Enumeration](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [Impacket](#) &emsp;|&emsp;  [NetDom](#) &emsp;|&emsp;  [Dcom](#)<br />

- **Kerberoasting :&emsp;** Extract service tickets to crack passwords.
    - ***Tools &emsp; =>*** &emsp; [Kerberoast](#) &emsp;|&emsp;  [Rubeus](#) &emsp;|&emsp;  [Impacket](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [PowerView](#) &emsp;|&emsp;  [BloodHound](#) &emsp;|&emsp;  [GetNPUsers](#) &emsp;|&emsp;  [Kerbrute](#) &emsp;|&emsp;  [Kerberoast](#) &emsp;|&emsp;  [GetUserSPNs](#)<br />

- **SPN Enumeration :&emsp;** Discover Service Principal Names.
    - ***Tools &emsp; =>*** &emsp; [Kerberoast](#) &emsp;|&emsp;  [Rubeus](#) &emsp;|&emsp;  [Impacket](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [PowerView](#) &emsp;|&emsp;  [BloodHound](#) &emsp;|&emsp;  [GetNPUsers](#) &emsp;|&emsp;  [Kerbrute](#) &emsp;|&emsp;  [GetUserSPNs](#) &emsp;|&emsp;  [Kerberoast](#)<br />

- **Kerberos Ticket Extraction :&emsp;** Obtain Kerberos tickets for analysis.
    - ***Tools &emsp; =>*** &emsp; [Rubeus](#) &emsp;|&emsp;  [Impacket](#) &emsp;|&emsp;  [Kerberoast](#) &emsp;|&emsp;  [GetNPUsers](#) &emsp;|&emsp;  [CrackMapExec](#) &emsp;|&emsp;  [PowerView](#) &emsp;|&emsp;  [BloodHound](#) &emsp;|&emsp;  [Kerbrute](#) &emsp;|&emsp;  [Kerberoast](#) &emsp;|&emsp;  [Mimikatz](#)

## 6. Privilege Escalation Techniques
1.  - ***Tools &emsp; =>*** &emsp; [Fuzzy Security Guide](https://www.fuzzysecurity.com/tutorials/16.html) &emsp;|&emsp; [PayloadsAllTheThings Guide](https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/Windows%20-%20Privilege%20Escalation.md) &emsp;|&emsp; [Absolomb Windows Privilege Escalation Guide](https://www.absolomb.com/2018-01-26-Windows-Privilege-Escalation-Guide/) &emsp;|&emsp; [Sushant 747's Guide (Country dependant - may need VPN)](https://sushant747.gitbooks.io/total-oscp-guide/content/privilege_escalation_windows.html) &emsp;|&emsp; [All resources used in the course](https://github.com/Gr1mmie/Windows-Priviledge-Escalation-Resources)

### 6.1 Linux Privilege Escalation<br />

- **SUID/SGID Files :&emsp;** Identify files with SUID or SGID permissions.
    - ***Tools &emsp; =>*** &emsp; [find](#) &emsp;|&emsp;  [LinPeas](#) &emsp;|&emsp;  [Linux Exploit Suggester](#) &emsp;|&emsp;  [GTFOBins](#) &emsp;|&emsp;  [LinEnum](#) &emsp;|&emsp;  [Pspy](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [RogueMaster](#) &emsp;|&emsp;  [Linux Privilege Escalation Scripts](https://github.com/sullo/kerberoasting)<br />

- **Kernel Exploits :&emsp;** Check for vulnerabilities in the Linux kernel.
    - ***Tools &emsp; =>*** &emsp; [uname](#) &emsp;|&emsp;  [Kernel Exploits](#) &emsp;|&emsp;  [Linux Exploit Suggester](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [Exploit-DB](https://www.exploit-db.com/)<br />

- **Cron Jobs :&emsp;** Identify misconfigured cron jobs.
    - ***Tools &emsp; =>*** &emsp; [crontab](#) &emsp;|&emsp;  [LinPeas](#) &emsp;|&emsp;  [Linux Exploit Suggester](#) &emsp;|&emsp;  [GTFOBins](#) &emsp;|&emsp;  [LinEnum](#) &emsp;|&emsp;  [Pspy](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [RogueMaster](#) &emsp;|&emsp;  [Linux Privilege Escalation Scripts](https://github.com/sullo/kerberoasting)<br />

- **Writable Directories :&emsp;** Check for directories where files can be written.
    - ***Tools &emsp; =>*** &emsp; [find](#) &emsp;|&emsp;  [LinPeas](#) &emsp;|&emsp;  [Linux Exploit Suggester](#) &emsp;|&emsp;  [GTFOBins](#) &emsp;|&emsp;  [LinEnum](#) &emsp;|&emsp;  [Pspy](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [RogueMaster](#) &emsp;|&emsp;  [Linux Privilege Escalation Scripts](https://github.com/sullo/kerberoasting)<br />

- **Environment Variables :&emsp;** Inspect environment variables for sensitive data.
    - ***Tools &emsp; =>*** &emsp; [env](#) &emsp;|&emsp;  [printenv](#) &emsp;|&emsp;  [LinPeas](#) &emsp;|&emsp;  [Linux Exploit Suggester](#) &emsp;|&emsp;  [GTFOBins](#) &emsp;|&emsp;  [LinEnum](#) &emsp;|&emsp;  [Pspy](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [RogueMaster](#) &emsp;|&emsp;  [Linux Privilege Escalation Scripts](https://github.com/sullo/kerberoasting)<br />

- **SetUID Binaries :&emsp;** Check for binaries with SetUID permissions.
    - ***Tools &emsp; =>*** &emsp; [find](#) &emsp;|&emsp;  [LinPeas](#) &emsp;|&emsp;  [Linux Exploit Suggester](#) &emsp;|&emsp;  [GTFOBins](#) &emsp;|&emsp;  [LinEnum](#) &emsp;|&emsp;  [Pspy](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [RogueMaster](#) &emsp;|&emsp;  [Linux Privilege Escalation Scripts](https://github.com/sullo/kerberoasting)<br />

- **Sudo Permissions :&emsp;** Inspect sudo permissions and configurations.
    - ***Tools &emsp; =>*** &emsp; [sudo -l](#) &emsp;|&emsp;  [LinPeas](#) &emsp;|&emsp;  [Linux Exploit Suggester](#) &emsp;|&emsp;  [GTFOBins](#) &emsp;|&emsp;  [LinEnum](#) &emsp;|&emsp;  [Pspy](#) &emsp;|&emsp;  [Enum4linux](#) &emsp;|&emsp;  [RogueMaster](#)

### 6.2 Windows Privilege Escalation<br />

- **Unquoted Service Paths :&emsp;** Identify unquoted service paths that can be exploited.
    - ***Tools &emsp; =>*** &emsp; [wmic](#) &emsp;|&emsp;  [PowerShell](#) &emsp;|&emsp;  [Sysinternals](#) &emsp;|&emsp;  [Accesschk](#) &emsp;|&emsp;  [Procmon](#) &emsp;|&emsp;  [Autoruns](#) &emsp;|&emsp;  [WinPEAS](#) &emsp;|&emsp;  [Windows Exploit Suggester](#) &emsp;|&emsp;  [Metasploit](#)<br />

- **Insecure File Permissions :&emsp;** Check for files with insecure permissions.
    - ***Tools &emsp; =>*** &emsp; [icacls](#) &emsp;|&emsp;  [Accesschk](#) &emsp;|&emsp;  [WinPEAS](#) &emsp;|&emsp;  [Sysinternals](#) &emsp;|&emsp;  [PowerShell](#) &emsp;|&emsp;  [Windows Exploit Suggester](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Dirbuster](#)<br />

- **Local Privilege Escalation Vulnerabilities :&emsp;** Look for known local privilege escalation vulnerabilities.
    - ***Tools &emsp; =>*** &emsp; [WinPEAS](#) &emsp;|&emsp;  [Windows Exploit Suggester](#) &emsp;|&emsp;  [PowerShell](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [Exploit-DB](#) &emsp;|&emsp;  [CVE Details](#) &emsp;|&emsp;  [MSFvenom](#) &emsp;|&emsp;  [MSFconsole](#)<br />

- **Scheduled Tasks :&emsp;** Check for tasks that can be exploited for privilege escalation.
    - ***Tools &emsp; =>*** &emsp; [schtasks](#) &emsp;|&emsp;  [PowerShell](#) &emsp;|&emsp;  [Sysinternals](#) &emsp;|&emsp;  [WinPEAS](#) &emsp;|&emsp;  [Accesschk](#) &emsp;|&emsp;  [Task Scheduler](#) &emsp;|&emsp;  [Scheduled Tasks Explorer](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Netcat](#)<br />

- **Kerberos Ticket Extraction :&emsp;** Obtain Kerberos tickets to elevate privileges.
    - ***Tools &emsp; =>*** &emsp; [Rubeus](#) &emsp;|&emsp;  [Mimikatz](#) &emsp;|&emsp;  [PowerView](#) &emsp;|&emsp;  [Impacket](#) &emsp;|&emsp;  [GetNPUsers](#) &emsp;|&emsp;  [Kerberoast](#) &emsp;|&emsp;  [Kerbrute](#) &emsp;|&emsp;  [BloodHound](#) &emsp;|&emsp;  [PowerSploit](#) &emsp;|&emsp;  [Metasploit](#)<br />

- **Service Account Misconfigurations :&emsp;** Identify misconfigured service accounts.
    - ***Tools &emsp; =>*** &emsp; [PowerView](#) &emsp;|&emsp;  [BloodHound](#) &emsp;|&emsp;  [WinPEAS](#) &emsp;|&emsp;  [Nmap](#) &emsp;|&emsp;  [Netcat](#) &emsp;|&emsp;  [PowerShell](#) &emsp;|&emsp;  [Service Account Finder](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [Windows Exploit Suggester](#) &emsp;|&emsp;  [Sysinternals](#)<br />

- **DLL Hijacking :&emsp;** Exploit DLL hijacking vulnerabilities for privilege escalation.
    - ***Tools &emsp; =>*** &emsp; [DLL Hijacking](#) &emsp;|&emsp;  [PowerShell](#) &emsp;|&emsp;  [Sysinternals](#) &emsp;|&emsp;  [Metasploit](#) &emsp;|&emsp;  [WinPEAS](#) &emsp;|&emsp;  [Accesschk](#)

- **Kernel Exploits**
    - ***Tools &emsp; =>*** &emsp; [Windows Kernel Exploits](https://github.com/SecWiki/windows-kernel-exploits)

### 6.3 Automated Tools for Privilege Escalation <br />

- **Unquoted Service Paths :&emsp;** Identify unquoted service paths that can be exploited.
    - ***Tools &emsp; =>*** &emsp; [WinPEAS](https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite/tree/master/winPEAS) &emsp;|&emsp; [Windows PrivEsc Checklist](https://book.hacktricks.xyz/windows/checklist-windows-privilege-escalation) &emsp;|&emsp; [Sherlock](https://github.com/rasta-mouse/Sherlock) &emsp;|&emsp; [Watson](https://github.com/rasta-mouse/Watson) &emsp;|&emsp; [PowerUp](https://github.com/PowerShellMafia/PowerSploit/tree/master/Privesc) &emsp;|&emsp; [JAWS](https://github.com/411Hall/JAWS) &emsp;|&emsp; [Windows Exploit Suggester](https://github.com/AonCyberLabs/Windows-Exploit-Suggester) &emsp;|&emsp; [Metasploit Local Exploit Suggester](https://blog.rapid7.com/2015/08/11/metasploit-local-exploit-suggester-do-less-get-more/) &emsp;|&emsp; [Seatbelt](https://github.com/GhostPack/Seatbelt) &emsp;|&emsp; [SharpUp](https://github.com/GhostPack/SharpUp)


## Metasploit Exploitation
- ***Tools &emsp; =>*** &emsp; [Kitrap0d Information](https://seclists.org/fulldisclosure/2010/Jan/341)

## Manual Kernel Exploitation
- ***Tools &emsp; =>*** &emsp; [MS10-059 Exploit](https://github.com/SecWiki/windows-kernel-exploits/tree/master/MS10-059)

## Gaining a Foothold
- ***Tools &emsp; =>*** &emsp; [Achat Exploit](https://www.exploit-db.com/exploits/36025) &emsp;|&emsp; [Achat Exploit (Metasploit)](https://www.rapid7.com/db/modules/exploit/windows/misc/achat_bof) &emsp;|&emsp; [Groovy Reverse Shell](https://gist.github.com/frohoff/fed1ffaab9b9beeb1c76)

## Escalation via Stored Passwords
- ***Tools &emsp; =>*** &emsp; [Plink Download](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

## Escalation via WSL
- ***Tools &emsp; =>*** &emsp; [Spawning a TTY Shell](https://netsec.ws/?p=337) &emsp;|&emsp; [Impacket Toolkit](https://github.com/SecureAuthCorp/impacket)

## Potato Attacks
- ***Tools &emsp; =>*** &emsp; [Rotten Potato](https://foxglovesecurity.com/2016/09/26/rotten-potato-privilege-escalation-from-service-accounts-to-system/) &emsp;|&emsp; [Juicy Potato](https://github.com/ohpe/juicy-potato)

## Impersonation and Alternate Data Streams
- ***Tools &emsp; =>*** &emsp; [Alternate Data Streams](https://blog.malwarebytes.com/101/2015/07/introduction-to-alternate-data-streams/)

## getsystem Overview
- ***Tools &emsp; =>*** &emsp; [What happens when I type getsystem?](https://blog.cobaltstrike.com/2014/04/02/what-happens-when-i-type-getsystem/)

## Startup Applications
- ***Tools &emsp; =>*** &emsp; [icacls Documentation](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/icacls)

## CVE-2019-1388 Overview
- ***Tools &emsp; =>*** &emsp; [Zero Day Initiative CVE-2019-1388](https://www.youtube.com/watch?v=3BQKpPNlTSo) &emsp;|&emsp; [Rapid7 CVE-2019-1388](https://www.rapid7.com/db/vulnerabilities/msft-cve-2019-1388)

## Challenge Walkthroughs
- ***Tools &emsp; =>*** &emsp; [Basic PowerShell for Pentesters](https://book.hacktricks.xyz/windows/basic-powershell-for-pentesters) &emsp;|&emsp; [Mounting VHD Files](https://medium.com/@klockw3rk/mounting-vhd-file-on-kali-linux-through-remote-share-f2f9542c1f25) &emsp;|&emsp; [Capturing MSSQL Credentials](https://medium.com/@markmotig/how-to-capture-mssql-credentials-with-xp-dirtree-smbserver-py-5c29d852f478)
