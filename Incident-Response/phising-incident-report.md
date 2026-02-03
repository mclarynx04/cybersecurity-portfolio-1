Phishing Incident Response Simulation
1. Objective
The objective of this project is to simulate and investigate a phishing
incident and document the response process as a SOC analyst.

 2. Tools Used
- Windows Event Viewer
- Sysmon
- Sample phishing logs

 3. Incident Overview
A simulated phishing attack was analyzed to determine how the attack
occurred, identify indicators of compromise, and assess potential impact.

 4. Investigation Steps
 Reviewed the reported phishing email for suspicious indicators
- Analyzed sender email address and domain reputation
- Examined embedded URL for signs of impersonation
- Confirmed user interaction with the phishing link
- Assessed potential credential compromise

 5. Findings
- The email was confirmed to be aphising attempt impersonating Microsoft
- The sender domain was not associated with legitimate Microsoft services
- The embedde URL redirected to a fake login page
- User credentials were potentially compromised after submission

 6. Indicators of Compromise (IOCs)
- malicious sender domain: m1crosoft-secure.com
- Phishing URL: http://microsoft-login-secure.co/verify
- Email subject: Urgent Unusual Sign-in Activity Detected

 7. Lessons Learned
User should be trained to verify sender domians before clicking links
Urgent language is a common phishing link
Multi-factor authentication can reduce the impact of credential theft
Early reporting helps reduce damage from phishing attacks.

 8. MITRE ATTACK Mapping

| Tactic | Technique ID | Technique Name | Description |
|--------|--------------|----------------|-------------|
| Initial Access | T1566 | Phishing | The attacker used a phishing email to trick the user into providing credentials |
| Credential Access | T1056 | Input Capture | User credentials were captured through a fake login page |

