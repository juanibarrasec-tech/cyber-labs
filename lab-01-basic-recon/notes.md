# Lab 01 – Notes & Findings

## 1. Passive Reconnaissance  
Initial review of the target using a browser and public DNS tools.

Observations:  
- Domain is active and reachable  
- No exposed sensitive information on the homepage  
- Standard web technologies detected

---

## 2. DNS Resolution  
Command used:  
```bash  
nslookup example.com
```

Result:
- Domain resolves successfully
- Multiple IP addresses returned (expected behavior)  

---

## 3. Connectivity Test
Command used:
```bash
ping example.com
```

Result:
- Host reachable
- Stable response times
- No packet loss observed  

---

## 4. Basic Port Scan
Command used:
```bash
nmap -F example.com
```

Observed open ports:
- 80 (HTTP)
- 443 (HTTPS)  

No unusual services detected.  

---

## 5. Analysis
- Target exposes only expected services
- No misconfigurations observed
- Behavior consistent with a public demonstration domain  

---

## 6. Conclusion
Reconnaissance phase completed successfully. No exploitation attempted. Information gathered is minimal and expected.

Key learning:
- Recon is about observation, not attack
- Documentation is as important as execution
