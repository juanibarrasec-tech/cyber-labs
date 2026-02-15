# Lab 02 – Enumeration Notes

## 1. Target Validation  
Before enumeration, confirmed that the target is a public testing host.

Target: scanme.nmap.org

---

## 2. Port and Service Detection  
Command used:  
```bash  
nmap -sV scanme.nmap.org
```

Observed services:
- 22 (SSH)
- 80 (HTTP)
- Other standard services may appear depending on scan time  

Service version detection enabled using safe parameters.  

---

## 3. Banner Observation
Nmap output provided basic service banners. No manual banner grabbing performed.  

---

## 4. Web Enumeration (Light)
- Accessed HTTP service via browser
- Observed default pages
- No directory brute forcing performed  

---

## 5. Analysis
- Services exposed are expected for a test environment
- No misconfigurations identified during basic enumeration
- Enumeration increases visibility compared to simple recon  

---

## 6. Key Differences from Recon
- Enumeration focuses on details
- Reveals versions and service behavior
- Still non-intrusive when done correctly  

---

## 7. Conclusion
Enumeration completed successfully. No exploitation attempted. Documentation reflects observed data only.

Key learning: Enumeration bridges recon and exploitation but must remain controlled.
