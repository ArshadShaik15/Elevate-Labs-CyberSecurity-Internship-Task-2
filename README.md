# Elevate-Labs-CyberSecurity-Internship-Task-2

<br>

### Task 2: Analyze a Phishing Email Sample
<br>

### **Phishing Threat Analysis:** <br>

This report analyzes two distinct email samples impersonating Cisco/Webex to demonstrate two primary social engineering tactics: <br>
1. Fear/Urgency (Threat-Based) <br>
2. Lure/Attract (Reward-Based) <br>
<br>

### **🎯 Objective:** <br>

The primary objective of this task is to identify and document the characteristics of a phishing attack within a suspicious email sample in order to build a solid awareness of phishing tactics and essential email threat analysis skills.  <br>
<br>
<br>
### **🛠️ Lab Setup:**  <br><br>
### **📝 Note:**  <br>

I originally wanted to download the native email files, known as **.eml** (email message) files, because they contain all the technical details, like the full hidden headers. But downloading unverified .eml files is very dangerous. They can carry active, hidden viruses or malicious code (payloads) that could run automatically on my system. This high risk of code execution made the direct download unsafe.
<br>
<br>

### **Obtaining a Sample Phishing Email:**  <br>

&nbsp;• I have tried downloading the the html format of the sample phishing mails from online.For further reference you can check for the  <br>  &nbsp; "HTML Files" folder. <br>
&nbsp;•  For further reference you can check for the "HTML Files" folder. <br>
<br>

### **Tools Recommended:** <br>

•  **MXToolbox** <br>
&nbsp; MXToolbox https://mxtoolbox.com/ is a popular, free online suite of tools used by IT and cybersecurity professionals to diagnose, monitor, <br> &nbsp; and troubleshoot email infrastructure and domain health. <br>

•  **MXToolbox Header Analyzer** <br>
&nbsp; The MXToolbox Email Header Analyzer https://mxtoolbox.com/EmailHeaders.aspx (or similar online tools) is a utility specifically designed to <br> &nbsp; decode and interpret the full email header. <br>

•  **EML Analyzer** <br>
&nbsp; An EML Analyzer https://eml-analyzer.herokuapp.com/#/ is typically a more comprehensive tool focused on digital forensics, designed to <br> &nbsp; examine a saved email file (an .eml file) to extract and display all its components and metadata for investigation. <br>
<br>
<br>

## **📧 Analysis of Cisco_Account_Suspension.html: Threat-Based Social Engineering** <br>
<br>

### &nbsp;**Step-1: Examining Sender's Email Address For Spoofing:** <br>

<br>  <img width="1650" height="870" alt="Screenshot 2025-10-22 182045" src="https://github.com/user-attachments/assets/c4bd01e7-e843-471a-b78d-cef72602e26f" />  <br>
<br>
&nbsp;•  The "From:" field uses a look-alike domain: "Cisco IT-Help Desk" <it-security@ciscoteam.com>. <br>
&nbsp;•  This is a clear instance of Domain Impersonation, as the official domain (cisco.com) is not used. <br>
<br>

### &nbsp;**Step-2: Checking Email Headers For Discrepancies:** <br>

<br>  <img width="1641" height="948" alt="Screenshot 2025-10-22 174013" src="https://github.com/user-attachments/assets/31113b93-359f-49cc-8275-e9aefe9304db" />  <br>
<br>
&nbsp;•  Full headers for external analysis are not available from the HTML content. <br>
&nbsp;•  However, the use of the unofficial domain **(@ciscoteam.com)** in the "From:" header is a major discrepancy. <br>
<br>

&nbsp;**Step-3: Identifying Suspicious Links or Attachments:** <br>

<br>  <img width="1649" height="868" alt="Screenshot 2025-10-22 185000" src="https://github.com/user-attachments/assets/afbf6fb3-2e9f-4b73-879b-2517a9eb1b12" />  <br>
<br>
&nbsp;•  It uses a single, prominent call-to-action link, "Verify My Account Now". But there were no attachments included. <br>
<br>

&nbsp;**Step-4: Look For Urgent Or Threatening :Language In The Email Body:** <br>

<br>  <img width="1649" height="873" alt="Screenshot 2025-10-22 182639" src="https://github.com/user-attachments/assets/4a07c97f-3b8b-4477-8683-6728fe108c0d" />  <br>
<br>  <img width="1642" height="864" alt="Screenshot 2025-10-22 191639" src="https://github.com/user-attachments/assets/c63fde0e-a41d-44f5-bc09-0565b4ca4b81" />  <br>
<br>
&nbsp;•  The header consists of the "Subject:" field which uses "Urgent: Action Required for Your Cisco Account". <br>
&nbsp;•  The body employs aggressive, fear-based social engineering with phrases like "temporarily suspended," "unauthorized login attempt," and  <br> &nbsp;&nbsp; the critical ultimatum: "permanently disabled for security reasons" if action is not taken within 24 hours. <br>
