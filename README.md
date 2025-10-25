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

<p align="left">I originally wanted to download the native email files, known as <strong>.eml</strong> (email message) files, because they contain all the technical details, like the full hidden headers. But downloading unverified .eml files is very dangerous. They can carry active, hidden viruses or malicious code (payloads) that could run automatically on my system. This high risk of code execution made the direct download unsafe. </p>
<br>
<br>

### **Obtaining a Sample Phishing Email:**  <br>

&nbsp;• I have downloaded the html format of the sample phishing mails from online. <br>
&nbsp;•  For further reference you can check for the "HTML Files" section. <br>
<br>

### **Tools Recommended:** <br>

•  **MXToolbox Header Analyzer** <br>
<p align="left"> &nbsp;The MXToolbox Email Header Analyzer https://mxtoolbox.com/EmailHeaders.aspx (or similar online tools) is a utility specifically designed to decode and interpret the full email header. <br> </p>

•  **EML Analyzer** <br>
<p align="left"> &nbsp;An EML Analyzer https://eml-analyzer.herokuapp.com is typically a more comprehensive tool focused on digital forensics, designed to examine a saved email file (an .eml file) to extract and display all its components and metadata for investigation. <br> </p>
<br>
<br>
<br>

## **📧 Analysis of Cisco_Account_Suspension.html: Threat-Based Social Engineering** <br>
<br>

<p align="left"> <strong>Phishing Type:</strong> Account Suspension / Credential Harvest (Fear-Based Attack) <br>
<strong>Primary Goal:</strong> Force the recipient into entering login credentials under the immediate threat of account deactivation. <br> </p>
<br>

### &nbsp;**Step-1: Examining Sender's Email Address For Spoofing:** <br>

<br>  <img width="1650" height="870" alt="Screenshot 2025-10-22 182045" src="https://github.com/user-attachments/assets/c4bd01e7-e843-471a-b78d-cef72602e26f" />  <br>
<br>
&nbsp;•  The "From:" field uses a look-alike domain: "Cisco IT-Help Desk" <it-security@ciscoteam.com> <br>
&nbsp;•  This is a clear instance of Domain Impersonation, as the official domain <strong>(cisco.com)</strong> is not used. <br>
<br>

### &nbsp;**Step-2: Checking Email Headers For Discrepancies:** <br>

<br>  <img width="1641" height="948" alt="Screenshot 2025-10-22 174013" src="https://github.com/user-attachments/assets/31113b93-359f-49cc-8275-e9aefe9304db" />  <br>
<br>
<p align="left"> &nbsp;•  Full headers for external analysis are not available from the HTML content. <br>
&nbsp;•  However, the use of the unofficial domain <strong>(@ciscoteam.com)</strong> in the "From:" header is a major discrepancy. <br> </p>
<br>

### &nbsp;**Step-3: Identifying Suspicious Links or Attachments:** <br>

<br>  <img width="1649" height="868" alt="Screenshot 2025-10-22 185000" src="https://github.com/user-attachments/assets/afbf6fb3-2e9f-4b73-879b-2517a9eb1b12" />  <br>
<br>
<p align="left"> &nbsp;•  It uses a single, prominent call-to-action link, "Verify My Account Now". But there were no attachments included. <br> </p>
<br>

### &nbsp;**Step-4: Look For Urgent Or Threatening :Language In The Email Body:** <br>

<br>  <img width="1649" height="873" alt="Screenshot 2025-10-22 182639" src="https://github.com/user-attachments/assets/4a07c97f-3b8b-4477-8683-6728fe108c0d" />  <br>
<br>  <img width="1642" height="864" alt="Screenshot 2025-10-22 191639" src="https://github.com/user-attachments/assets/c63fde0e-a41d-44f5-bc09-0565b4ca4b81" />  <br>
<br>
<p align="left"> &nbsp;•  The header consists of the "Subject:" field which uses "Urgent: Action Required for Your Cisco Account". <br>
&nbsp;•  The body employs aggressive, fear-based social engineering with phrases like "temporarily suspended", "unauthorized login attempt", and the critical ultimatum: "permanently disabled for security reasons" if action is not taken within 24 hours. <br> </p>
<br>

### &nbsp;**Step-5: Noting down the mismatched URLs:** <br>

<br>  <img width="1647" height="866" alt="Screenshot 2025-10-22 193143" src="https://github.com/user-attachments/assets/2f888712-09e0-458d-a420-ac46a36d0def" />  <br>
<br>
<p align="left"> &nbsp;•  The display text is simialr ("Verify My Account Now"), but the embedded payload URL is http://webex-cisco-verify.com/login <br>
&nbsp;•  This is a look-alike domain designed for credential harvesting, and the use of the unsecured HTTP protocol is a significant technical indicator of compromise. <br> </p>
<br>

### &nbsp;**Step-6: Verify presence of spelling or grammar errors:** <br>

<p align="left"> &nbsp;•  The text maintains high composition quality and is free of common errors. <br>
&nbsp;•  This indicates the phishing attempt was crafted by a sophisticated threat group, which significantly enhances the email's perceived legitimacy and effectiveness. <br> </p>
<br>
<br>
<br>

## **📧 Analysis of Cisco_Webex_Subscription.html: Reward-Based Social Engineering** <br>
<br>

### &nbsp;**Step-1: Examining Sender's Email Address For Spoofing:** <br>

<br>    <img width="1053" height="777" alt="Screenshot 2025-10-22 200120" src="https://github.com/user-attachments/assets/6590ca77-8e2e-4c18-aaec-62f0aab0190a" />    <br>
<br>
<p align="left"> &nbsp;•  The provided HTML body indicates the sender is "The Webex Team." This is an act of Brand Impersonation used to establish trust. <br> 
&nbsp;•  Though the actual sender email address is not visible in the HTML content provided. <br> </p>
<br>

### &nbsp;**Step-2: Checking Email Headers For Discrepancies:** <br>

<p align="left"> &nbsp;•  No headers are available in the provided HTML file content, preventing a full header analysis. <br> </p>
<br>

### &nbsp;**Step-3: Identifying Suspicious Links or Attachments:** <br>

<p align="left"> &nbsp;•  The primary focus is a single, enticing CTA (Call-to-Action) link: "Claim Your Free Year of Webex Pro Now!" No attachments were found. <br> </p>
<br>

### &nbsp;**Step-4: Look For Urgent Or Threatening :Language In The Email Body:** <br>

<br>    <img width="1083" height="744" alt="Screenshot 2025-10-22 201819" src="https://github.com/user-attachments/assets/9fc9b69a-7b17-4dd5-b0cc-d163960aa44e" />    <br>
<br>
<p align="left"> &nbsp;•  The email uses a language form of urgency based on <strong>Fear of Missing Out (FOMO)</strong> a <strong>high-value lure ("FREE 1-year subscription")</strong> and a <strong>sense of haste ("limited time," "Act fast")</strong> to pressure the user into immediate action. <br> </p>
<br>

### &nbsp;**Step-5: Noting down the mismatched URLs:** <br>

<p align="left"> &nbsp;•  The link text promises a claim, but the destination URL is the generic, suspicious placeholder {{.URL}}. This is a clear indicator that the email is a template used in a malicious campaign. <br> </p>
<br>

### &nbsp;**Step-6: Verify presence of spelling or grammar errors:** <br>

<br>     <img width="1107" height="763" alt="Screenshot 2025-10-22 203009" src="https://github.com/user-attachments/assets/03416bce-35ad-42dd-8540-f10853e385da" />    <br>
<br>
<p align="left"> &nbsp;•  The body is well formatted and the text is professionally written and lacks obvious spelling or grammar errors, indicating a more sophisticated attempt. <br> </p> 
<p align="left"> &nbsp;•  Interestingly, it includes a false disclaimer ("Beware of phishing scams") in the footer, a tactic used to establish deceptive credibility. </p> 
<br>
<br>
<br>

### Summarizing The Phishing Traits Found In Both The Emails: <br>

This campaign utilizes two sophisticated phishing email templates impersonating Cisco/Webex services, both designed for credential harvesting.The first sample **(Cisco_Account_Suspension.html)** employs Fear-Based Social Engineering, using explicit threats of permanent account deactivation and a 24-hour deadline to trigger panic. The second sample **(Cisco_Webex_Subscription.html)** employs Reward-Based Social Engineering, using a high-value lure (a "Free Pro Subscription") to exploit the recipient's curiosity and sense of FOMO (Fear of Missing Out). Both samples use brand impersonation, high-quality text composition, and rely on non-official or dynamically inserted payload URLs to bypass security filters and steal login credentials.<br>
<br>
This table summarizes the most critical Indicators of Compromise (IoCs) found across both samples <br>
<br>

| Indicator                | Location in Email                                                                 | Severity |
|---------------------------|----------------------------------------------------------------------------------|-----------|
| Spoofed Sender Domain     | From: field in Threat-Based sample (@ciscoteam.com)                              | **🔴 CRITICAL** |
| Payload URL (Look-alike)  | Link in Threat-Based sample (webex-cisco-verify.com)                             | **🔴 CRITICAL** |
| Unsecured Protocol        | Link in Threat-Based sample uses http:// (unencrypted)                           | **🟠 HIGH**     |
| Extreme Urgency/Threat    | Subject (Urgent: Action Required...) and body (24-hour deadline)                 | **🟠 HIGH**     |
| Malicious URL Placeholder | Link in Reward-Based sample ({{.URL}})                                           | **🟠 HIGH**     |
| High-Value Lure           | Body of Reward-Based sample (Promise of "Free Year of Webex Pro")                | **🟡 MODERATE** |
| Deceptive Credibility     | Footer of Reward-Based sample (Fake anti-phishing disclaimer)                    | **🟡 MODERATE** |
<br>

| Phishing Type                              | Tactic Used                                                                                     | Goal (Psychological Mechanism)                                                                                             |
|--------------------------------------------|--------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|
| Fear and Urgency (Threat-Based Phish)      | Threatens the immediate, negative loss of a vital service (e.g., permanent account deactivation). | Triggers an emotional, panic-driven response, causing the user to bypass logical security checks (like verifying the URL). |
| Attraction and Curiosity (Reward-Based Phish) | Lures the user with a valuable reward ("FREE Pro Subscription") or a limited-time opportunity (FOMO). | Exploits greed or curiosity to drive clicks. The user is motivated to act quickly before the perceived offer expires.      |
<br>
<br>


### **Conclusion:** <br>

<p align="left"> The analysis confirms a sophisticated, dual-pronged Social Engineering campaign targeting our digital assets for Credential Harvesting. The threat is structured around two key psychological drivers: Fear (leveraged by the Threat-Based Phish using Urgency and explicit threats of permanent deactivation) and Greed (leveraged by the Reward-Based Phish using High-Value Lures and FOMO). Both attacks rely on the technical flaw of Domain Impersonation (e.g., ciscoteam.com) and the use of Malicious Payload URLs to steal user login data. </p>
<p align="left"> To achieve a robust Security Posture, organizations must implement a layered Mitigation Strategy focused on both technical controls (e.g., blocking look-alike domains and unauthenticated senders at the gateway) and continuous User Awareness Training. The primary defense remains the end-user's adherence to the principle of "Stop, Look, and Manually Verify" by navigating directly to official service websites, thereby nullifying the effectiveness of any malicious link. </p> <br>

### **🛡️  Recommended Mitigation Strategy:** <br> 

| Action Category     | Recommended Steps                                                                                                                                          | Reason                                                                                                         |
|----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
| Immediate Response   | Mark as Phishing and delete both emails. Do **NOT** click any links.                                                                                       | Prevents exposure to the payload and notifies email security providers.                                          |
| Technical Blocks     | Block the Sender Domain (`ciscoteam.com`) at the email gateway. Block the payload IP address/domain (`webex-cisco-verify.com`) at the firewall/DNS level.   | Prevents all future emails from the threat actor using this infrastructure.                                      |
| User Education       | Update users immediately regarding the two tactics used: the **Account Suspension scam** and the **Free Reward scam**.                                    | Increases user awareness, turning human vulnerability into a strong line of defense.                            |
| Verification Policy  | Advise users to never click a link for sensitive actions (like account verification). Instead, manually navigate to the official **cisco.com** or **webex.com** website. | Establishes a secure habit that defeats look-alike domain attacks.                                               |
| Zero-Trust Verification  | Never trust the link. Adopt a strict policy: If an email requests sensitive action (like password resets or verification), do not click the link. Instead, manually type the official website address (cisco.com or webex.com) into your browser to verify the request. | The reason for the "Never trust the link" policy is that it completely eliminates the attacker's primary vector and relies on a trusted process rather than an untrusted element.
