# Answers to Assignment 8 Part 3

Add your answers to the questions in Assignment 8 Part 3, Step 2 below. 

## Vulernability Remediation:
### Vulnerability 1: 
**1. Which package or library are you addressing?**  
      PyYAML  
**2. Which CVE is linked to this vulnerability?**  
      CVE-2019-20477  
**3. What remediation steps do you suggest?**  
      CVE-2019-20477 is a critical vulnerability in PyYAML that allows for deserialization of untrusted data. This vulnerability could enable attackers to execute arbitrary code if untrusted YAML data is parsed.  
      Upgrade the PyYAML package to version 5.2 or higher, as this version contains the fix for the vulnerability. Additionally, avoid loading YAML data from untrusted sources, or if necessary, use safe loading methods such as yaml.safe_load() to prevent code execution from deserialized objects.
### Vulnerability 2:
**1. Which vulnerability are you addressing?**  
      Pillow  
**2. Which CVE is linked to this vulnerability?**  
      CVE-2023-4863  
**3. What remediation steps do you suggest?**  
      CVE-2023-4863 is a high-severity vulnerability in Pillow involving an out-of-bounds write, which could lead to denial of service or potential code execution when processing maliciously crafted image files.  
      Update the Pillow library to version 10.0.1 or higher, where this vulnerability is fixed. Also, ensure that only trusted image sources are used if possible, or sanitize user-uploaded images to reduce the risk of exploitation.
