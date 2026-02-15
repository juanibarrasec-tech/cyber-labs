# Lab 03 – Web Enumeration Notes

## 1. Initial Web Access  
Accessed the target using a standard web browser.

Observations:  
- Page loads correctly  
- No login forms present  
- No user input fields exposed

---

## 2. Page Source Review  
Reviewed HTML source code.

Findings:  
- Clean and minimal HTML structure  
- No embedded credentials  
- No commented sensitive data

---

## 3. HTTP Header Analysis  
Command used:  
```bash  
curl -I http://example.com
```

Observed headers:
- Server information
- Content-Type
- Cache-Control  

No unusual or sensitive headers identified.  

---

## 4. Technology Identification
Used browser developer tools to inspect:
- Network requests
- Response headers
- Basic technology indicators  

No client-side frameworks or exposed APIs detected.  

---

## 5. Light Automated Enumeration
Command used:
```bash
nmap --script http-headers example.com
```

Result:
- Confirmed previously observed headers
- No additional information exposed  

---

## 6. Analysis
- Web service behaves as expected for a public demo site
- No misconfigurations visible at this level
- Enumeration completed without intrusive actions  

---

## 7. Conclusion
Basic web enumeration completed successfully.

Key learning:
- Web enumeration relies heavily on observation
- Many useful details are available without attacking
- Documentation is critical for analysis and reporting
