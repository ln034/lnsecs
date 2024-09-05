# API Testing Checklist

## 1. Testing Approach <br />
- **Determine Testing Approach :&emsp;** Choose between black box, gray box, or white box testing based on the level of access and information available.<br />

## 2. Passive Reconnaissance <br />
- **Attack Surface Discovery :&emsp;** Identify all potential entry points and attack vectors.<br />
  - ***Tools &emsp; =>*** &emsp; [Shodan](#) &emsp;|&emsp; [Censys](#) &emsp;|&emsp; [Google Dorking](#) &emsp;|&emsp; [Recon-ng](#) &emsp;|&emsp; [BuiltWith](#)<br />
- **Exposed Secrets :&emsp;** Check for sensitive information such as API keys, tokens, and credentials that might be inadvertently exposed.<br />
  - ***Tools &emsp; =>*** &emsp; [GitHub Search](#) &emsp;|&emsp; [GitLab Search](#) &emsp;|&emsp; [TruffleHog](#) &emsp;|&emsp; [LeakCanary](#) &emsp;|&emsp; [DataLeaker](#)<br />

## 3. Active Reconnaissance <br />
- **Port and Service Scanning :&emsp;** Use tools to scan for open ports and services that may reveal additional endpoints or vulnerabilities.<br />
  - ***Tools &emsp; =>*** &emsp; [Nmap](#) &emsp;|&emsp; [Masscan](#) &emsp;|&emsp; [ZMap](#) &emsp;|&emsp; [Angry IP Scanner](#) &emsp;|&emsp; [Netcat](#)<br />
- **Application Usage :&emsp;** Interact with the application as an end-user to understand its behavior and API usage patterns.<br />
  - ***Tools &emsp; =>*** &emsp; [Browser DevTools](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Insomnia](#)<br />
- **Inspect with DevTools :&emsp;** Utilize browser developer tools to analyze network requests, responses, and JavaScript files.<br />
  - ***Tools &emsp; =>*** &emsp; [Chrome DevTools](#) &emsp;|&emsp; [Firefox Developer Tools](#) &emsp;|&emsp; [Edge DevTools](#) &emsp;|&emsp; [Fiddler](#) &emsp;|&emsp; [Burp Suite](#)<br />
- **API Directory Discovery :&emsp;** Search for directories related to the API, such as `/api/`, `/v1/`, or `/endpoints/`.<br />
  - ***Tools &emsp; =>*** &emsp; [DirBuster](#) &emsp;|&emsp; [Dirsearch](#) &emsp;|&emsp; [Gobuster](#) &emsp;|&emsp; [Wfuzz](#) &emsp;|&emsp; [Burp Suite](#)<br />
- **Endpoint Discovery :&emsp;** Identify all available API endpoints using tools.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [API Discovery Tools](#) &emsp;|&emsp; [API Fortress](#)<br />

## 4. Endpoint Analysis <br />
- **API Documentation Review :&emsp;** Locate and examine official API documentation or any available resources that describe the API’s functionality.<br />
  - ***Tools &emsp; =>*** &emsp; [Swagger UI](#) &emsp;|&emsp; [Redoc](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [API Blueprint](#) &emsp;|&emsp; [OpenAPI Specification](#)<br />
- **Reverse Engineering :&emsp;** Analyze the API's underlying structure to understand its implementation.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Fiddler](#) &emsp;|&emsp; [Charles Proxy](#)<br />
- **Use the API as Intended :&emsp;** Interact with the API based on its documented functionality to identify potential issues.<br />
  - ***Tools &emsp; =>*** &emsp; [Postman](#) &emsp;|&emsp; [Insomnia](#) &emsp;|&emsp; [cURL](#) &emsp;|&emsp; [HTTPie](#) &emsp;|&emsp; [SoapUI](#)<br />
- **Analyze Responses :&emsp;** Look for information disclosures, excessive data exposures, and business logic flaws.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Fiddler](#) &emsp;|&emsp; [Wireshark](#)<br />

## 5. Authentication Testing <br />
- **Basic Authentication Testing :&emsp;** Test for flaws in basic authentication mechanisms.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Nessus](#) &emsp;|&emsp; [Hydra](#)<br />
- **API Token Manipulation :&emsp;** Attempt to exploit and manipulate API tokens.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [JWT.io Debugger](#) &emsp;|&emsp; [Auth0](#) &emsp;|&emsp; [Burp Suite Extensions](#)<br />

## 6. Fuzzing <br />
- **Fuzz All Inputs :&emsp;** Use fuzzing techniques to test API inputs for unexpected behavior or vulnerabilities.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [AFL](#) &emsp;|&emsp; [Peach Fuzzer](#) &emsp;|&emsp; [Boofuzz](#)<br />

## 7. Authorization Testing <br />
- **Resource Identification Methods :&emsp;** Discover how resources are identified and accessed.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [API Testing Tools](#) &emsp;|&emsp; [Access Control Tester](#)<br />
- **Broken Object Level Authorization (BOLA) :&emsp;** Test for flaws in object-level access control.<br />
- **Broken Function Level Authorization (BFLA) :&emsp;** Test for flaws in function-level access control.<br />  
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [API Security Testing Tools](#) &emsp;|&emsp; [Manual Testing](#)<br />

## 8. Mass Assignment Testing <br />
- **Discover Standard Parameters :&emsp;** Identify parameters used in requests that might be susceptible to mass assignment attacks.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [API Testing Tools](#) &emsp;|&emsp; [Manual Testing](#)<br />
- **Test for Mass Assignment :&emsp;** Check if the API allows users to modify parameters that should be restricted.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [API Security Testing Tools](#) &emsp;|&emsp; [Manual Testing](#)<br />

## 9. Injection Testing <br />
- **User Input Testing :&emsp;** Discover and test requests that accept user input for injection vulnerabilities.<br />
  - ***Tools &emsp; =>*** &emsp; [SQLmap](#) &emsp;|&emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Commix](#) &emsp;|&emsp; [Fuzzing Tools](#)<br />
- **Test for XSS/XAS :&emsp;** Test for Cross-Site Scripting (XSS) and XML Injection vulnerabilities.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [XSSer](#) &emsp;|&emsp; [XSStrike](#) &emsp;|&emsp; [XML Injector](#)<br />
- **Database-Specific Attacks :&emsp;** Perform attacks tailored to specific database systems.<br />
  - ***Tools &emsp; =>*** &emsp; [SQLmap](#) &emsp;|&emsp; [MySQLi](#) &emsp;|&emsp; [NoSQLMap](#) &emsp;|&emsp; [PostgreSQL Tools](#) &emsp;|&emsp; [SQLNinja](#)<br />
- **Operating System Injection :&emsp;** Test for operating system command injection vulnerabilities.<br />
  - ***Tools &emsp; =>*** &emsp; [Commix](#) &emsp;|&emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Metasploit](#) &emsp;|&emsp; [Netcat](#)<br />

## 10. Rate Limit Testing <br />
- **Check for Rate Limits :&emsp;** Test if the API enforces rate limits to prevent abuse.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Rate Limit Tester](#) &emsp;|&emsp; [Wfuzz](#)<br />
- **Test Rate Limit Bypass Methods :&emsp;** Explore ways to bypass or evade rate limits.<br />
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Postman](#) &emsp;|&emsp; [Rate Limit Bypass Tools](#) &emsp;|&emsp; [Manual Testing](#)<br />

## 11. Evasive Techniques <br />
- **String Terminators :&emsp;** Add string terminators to payloads to test for evasion.<br />
- **Case Switching :&emsp;** Modify the case of payloads to bypass filters.<br />
- **Payload Encoding :&emsp;** Encode payloads to avoid detection.<br />
- **Combine Evasion Techniques :&emsp;** Use a combination of evasive techniques to increase effectiveness.<br />
- **Apply Evasion to All Tests :&emsp;** Ensure that evasive techniques are applied to all previous tests.<br />  
  - ***Tools &emsp; =>*** &emsp; [Burp Suite](#) &emsp;|&emsp; [OWASP ZAP](#) &emsp;|&emsp; [Fuzzing Tools](#) &emsp;|&emsp; [Custom Scripts](#) &emsp;|&emsp; [Manual Testing](#)<br />


