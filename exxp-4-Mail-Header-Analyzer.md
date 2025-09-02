# Experiment-4: Analyze Email Headers and Detect Email Spoofing Using Mail Header Analyzer

**Course / Lab:** Digital Forensics Lab  
**Experiment No.:** 4  
**Title:** Analyze Email Headers and Detect Email Spoofing Using Mail Header Analyzer  


---

## Aim
To analyze email headers and detect possible spoofing or malicious activity using Mail Header Analyzer.

---

## Requirements
- Mail Header Analyzer tool  
- Any email client (Gmail / Outlook / Yahoo) with suspicious email samples  

---

## Description
An email header contains routing information, including sender, recipient, subject, and most importantly, the path the email took across servers.  
Attackers often forge headers to trick recipients, called **email spoofing**.  

By analyzing headers, we can identify:  
- Real sender IP address  
- Authentication results (SPF, DKIM, DMARC)  
- Time delays between servers  
- Signs of spoofing / phishing  

---

## Procedure — Steps to Analyze Email Headers

**Step-1:** First, get the email header. In Gmail, select the mail, click the three dots, and choose **Show Original**.  


https://github.com/99230040236-byte/DF/blob/62b02fd1ef5a382d86d6b1f170f57eae27f15d76/exp1/Screenshot%20(38).png

**Step-2:** After clicking **Show Original**, you will see the raw message with sender and receiver details.  

https://github.com/99230040236-byte/DF/blob/62b02fd1ef5a382d86d6b1f170f57eae27f15d76/exp1/Screenshot%20(31).png
**Step-3:** Use the **Mail Header Analyzer tool** for easy reading and analysis.  

https://github.com/99230040236-byte/DF/blob/62b02fd1ef5a382d86d6b1f170f57eae27f15d76/exp1/Screenshot%20(32).png
**Step-4:** Copy and paste the entire header text into the tool and click **Analyze Header**.  


https://github.com/99230040236-byte/DF/blob/62b02fd1ef5a382d86d6b1f170f57eae27f15d76/exp1/Screenshot%20(34).png
**Step-5:** Identify key header fields:  
- From  
- To  
- Subject  
- Date  
- Return-Path  
- Received  
- Message-ID  
- SPF / DKIM / DMARC
  
https://github.com/99230040236-byte/DF/blob/62b02fd1ef5a382d86d6b1f170f57eae27f15d76/exp1/Screenshot%20(33).png
**Step-6:** Check for IP addresses and hostnames.  
- Use tools like **WHOIS** or online IP lookup services to identify the geographical location and ownership of IP addresses found in the *Received* lines.  
- Verify if any IPs are suspicious or if the hostname doesn’t match the expected sending server.

https://github.com/99230040236-byte/DF/blob/62b02fd1ef5a382d86d6b1f170f57eae27f15d76/exp1/Screenshot%20(37).png
**Step-7:** Examine the SPF, DKIM, and DMARC results:  
- **SPF (Sender Policy Framework):** Checks if the sender’s server/IP is authorized for that domain.  
- **DKIM (DomainKeys Identified Mail):** Ensures the email content wasn’t changed.  
- **DMARC (Domain-based Message Authentication, Reporting & Conformance):** Provides domain-level email authentication, policy, and reporting.

  
https://github.com/99230040236-byte/DF/blob/f0ce1dbb304ccbf7578aaa6200fc6721b87b8346/exp1/Screenshot%20(39).png

- SPF Sender Policy Framework → Checks if the sender’s server/IP is allowed for that
domain
- DKIM DomainKeys Identified Mail → Ensures email content wasn’t changed.

https://github.com/99230040236-byte/DF/blob/f0ce1dbb304ccbf7578aaa6200fc6721b87b8346/exp1/Screenshot%20(36).png

https://github.com/99230040236-byte/DF/blob/e1ca06dbd9c64f77809741107aee2795130657b0/exp1/Screenshot%20(40).png
---

## Expected Output
- The Mail Header Analyzer highlights key email header fields.  
- Authentication checks (SPF/DKIM/DMARC) show whether the email is genuine or spoofed.  
- Suspicious IP addresses or mismatched hostnames can be identified.  
- Email spoofing or phishing attempts are detected.  

---
