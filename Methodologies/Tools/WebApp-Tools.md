# Web Application Penetration Testing Checklist

## 1. Testing Approach <br />
- **Determine Testing Approach :&emsp;** Select between black box, gray box, or white box testing based on the level of access and information available.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Nessus](#) &emsp;|&emsp; [Veracode](#) &emsp;|&emsp; [SonarQube](#)<br />

## 2. Passive Reconnaissance <br />
- **Attack Surface Discovery :&emsp;** Identify and catalog all potential attack surfaces.<br />
  - ***Tools &emsp; =>*** &emsp; [Shodan](#) &emsp;|&emsp; [Censys](#) &emsp;|&emsp; [Google Dorking](#) &emsp;|&emsp; [Recon-ng](#) &emsp;|&emsp; [BuiltWith](#)<br />
- **Exposed Secrets :&emsp;** Look for exposed credentials, API keys, and other sensitive data.<br />
  - ***Tools &emsp; =>*** &emsp; [GitHub Search](#) &emsp;|&emsp; [GitLab Search](#) &emsp;|&emsp; [TruffleHog](#) &emsp;|&emsp; [LeakCanary](#) &emsp;|&emsp; [DataLeaker](#)<br />

## 3. Active Reconnaissance <br />
- **Port and Service Scanning :&emsp;** Identify open ports and running services to uncover potential vulnerabilities.<br />
  - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp; [Masscan](#) &emsp;|&emsp; [ZMap](#) &emsp;|&emsp; [Angry IP Scanner](#) &emsp;|&emsp; [Netcat](#)<br />
- **Web Application Interaction :&emsp;** Engage with the application to understand its functionality and uncover potential issues.<br />
  - ***Tools &emsp; =>*** &emsp; [Browser DevTools](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Insomnia](#)<br />
- **Inspect with DevTools :&emsp;** Use browser developer tools to analyze network traffic, cookies, and JavaScript.<br />
  - ***Tools &emsp; =>*** &emsp; [Chrome DevTools](#) &emsp;|&emsp; [Firefox Developer Tools](#) &emsp;|&emsp; [Edge DevTools](#) &emsp;|&emsp; [Fiddler](#) &emsp;|&emsp; [Burp Suite](#)<br />
- **Directory and File Discovery :&emsp;** Identify hidden directories and files that may reveal additional attack vectors.<br />
  - ***Tools &emsp; =>*** &emsp; [DirBuster](#) &emsp;|&emsp; [Dirsearch](#) &emsp;|&emsp; [Gobuster](#) &emsp;|&emsp; [Wfuzz](#) &emsp;|&emsp; [Nikto](#)<br />
- **Discover API Endpoints :&emsp;** Locate and test API endpoints for potential vulnerabilities.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [API Discovery Tools](#) &emsp;|&emsp; [API Fortress](#)<br />

## 4. Endpoint Analysis <br />
- **Review Web Application Documentation :&emsp;** Examine any available documentation for insights into the application’s functionality and potential weaknesses.<br />
  - ***Tools &emsp; =>*** &emsp; [Swagger UI](#) &emsp;|&emsp; [Redoc](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [OpenAPI Specification](#) &emsp;|&emsp; [Custom Documentation Review](#)<br />
- **Reverse Engineering :&emsp;** Analyze the application’s code and behavior to identify vulnerabilities.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Fiddler](#) &emsp;|&emsp; [Charles Proxy](#)<br />
- **Use the Application as Intended :&emsp;** Test the application’s functionality as a normal user to identify potential security issues.<br />
  - ***Tools &emsp; =>*** &emsp; [Postman](#) &emsp;|&emsp; [Insomnia](#) &emsp;|&emsp; [cURL](#) &emsp;|&emsp; [HTTPie](#) &emsp;|&emsp; [SoapUI](#)<br />
- **Analyze Responses :&emsp;** Review responses for information leaks, excessive data exposures, and potential business logic flaws.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Fiddler](#) &emsp;|&emsp; [Wireshark](#)<br />

## 5. Authentication Testing <br />
- **Basic Authentication Testing :&emsp;** Test the strength and security of basic authentication mechanisms.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Nessus](#) &emsp;|&emsp; [Hydra](#)<br />
- **Authentication Mechanism Testing :&emsp;** Evaluate various authentication mechanisms (e.g., OAuth, JWT) for vulnerabilities.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [JWT.io Debugger](#) &emsp;|&emsp; [Auth0](#) &emsp;|&emsp; [OAuth2 Proxy](#)<br />

## 6. Fuzzing <br />
- **Fuzz Input Fields :&emsp;** Apply fuzzing techniques to all input fields to identify unexpected behaviors and vulnerabilities.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [AFL](#) &emsp;|&emsp; [Peach Fuzzer](#) &emsp;|&emsp; [Boofuzz](#)<br />

## 7. Authorization Testing <br />
- **Resource Identification :&emsp;** Identify how resources are accessed and identified within the application.<br />
- **Test for Broken Access Control :&emsp;** Verify that access control mechanisms are implemented correctly and are resistant to exploitation.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Access Control Tester](#) &emsp;|&emsp; [API Security Testing Tools](#) &emsp;|&emsp; [Manual Testing](#)<br />

## 8. Mass Assignment Testing <br />
- **Identify Standard Parameters :&emsp;** Discover parameters used in requests that could be susceptible to mass assignment attacks.<br />
- **Test for Mass Assignment Vulnerabilities :&emsp;** Check if the application allows unauthorized modifications of parameters.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [API Security Testing Tools](#) &emsp;|&emsp; [Manual Testing](#)<br />

## 9. Injection Testing <br />
- **Identify Injection Points :&emsp;** Locate areas where user input could be processed and potentially vulnerable to injection attacks.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [SQLmap](#) &emsp;|&emsp; [Commix](#) &emsp;|&emsp; [Fuzzing Tools](#)<br />
- **Test for Cross-Site Scripting (XSS) :&emsp;** Assess the application for XSS vulnerabilities.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [XSSer](#) &emsp;|&emsp; [XSStrike](#) &emsp;|&emsp; [XSS Hunter](#)<br />
- **Test for SQL Injection :&emsp;** Evaluate input fields for SQL injection vulnerabilities.<br />
  - ***Tools &emsp; =>*** &emsp; [SQLmap](#) &emsp;|&emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [SQLNinja](#) &emsp;|&emsp; [SQLite Database Browser](#)<br />
- **Test for Command Injection :&emsp;** Identify vulnerabilities that allow for arbitrary command execution on the server.<br />
  - ***Tools &emsp; =>*** &emsp; [Commix](#) &emsp;|&emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Metasploit](#) &emsp;|&emsp; [Netcat](#)<br />

## 10. Rate Limit Testing <br />
- **Check for Rate Limits :&emsp;** Verify if the application enforces rate limits to mitigate abuse.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Rate Limit Tester](#) &emsp;|&emsp; [Wfuzz](#)<br />
- **Test Rate Limit Bypass :&emsp;** Explore techniques to bypass or evade rate limits.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Rate Limit Bypass Tools](#) &emsp;|&emsp; [Manual Testing](#)<br />

## 11. Evasive Techniques <br />
- **String Terminators :&emsp;** Add terminators to payloads to test evasion.<br />
- **Case Switching :&emsp;** Modify payload cases to bypass security filters.<br />
- **Payload Encoding :&emsp;** Use encoding techniques to evade detection.<br />
- **Apply Evasion to All Tests :&emsp;** Ensure evasive techniques are used across all testing phases.<br />
- **Combine Evasion Techniques :&emsp;** Apply a mix of evasion techniques for improved results.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Fuzzing Tools](#) &emsp;|&emsp; [Custom Scripts](#) &emsp;|&emsp; [Manual Testing](#)<br />

