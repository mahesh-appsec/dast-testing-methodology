# DAST Testing Methodology 🔍

A practical methodology for performing Dynamic Application Security Testing (DAST) across web applications using automated security scanning and manual security validation techniques.

This repository documents a structured DAST assessment lifecycle focused on identifying, validating and managing application security vulnerabilities.

---

## 🎯 Objective

The objective of DAST is to:

- Identify runtime application security vulnerabilities
- Analyze application behavior from an external perspective
- Validate security findings
- Reduce false positives
- Provide actionable remediation recommendations
- Verify remediation through security retesting

---

## 🔄 DAST Assessment Lifecycle

```text
Application Onboarding
          ↓
Scope & Configuration
          ↓
Application Walkthrough
          ↓
Authentication Setup
          ↓
Automated DAST Scan
          ↓
Finding Analysis
          ↓
Manual Validation
          ↓
False Positive Review
          ↓
Security Reporting
          ↓
Remediation Tracking


1️⃣ Application Onboarding
Before initiating a DAST assessment, the application should be onboarded based on the approved security assessment scope.
Onboarding Considerations
Application URL
Application environment
In-scope domains
Application architecture
Authentication requirements
Scan requirements
Testing restrictions

2️⃣ Scope & Scan Configuration
Proper scope definition and scan configuration are essential for effective DAST testing.
Configuration Considerations
Target URL
In-scope application paths
Excluded paths
Scan profile
Scan duration
Authentication configuration
Scanner location where applicable
Scan configuration should align with the approved assessment scope.

3️⃣ Application Walkthrough
A manual application walkthrough helps the security tester understand the application functionality and attack surface.
Key Areas
Application functionality
User roles
Authentication flow
Business workflows
Sensitive functionality
User input points
Application navigation
Understanding the application before scanning helps improve scan coverage and finding analysis.

4️⃣ Authentication Configuration
Authenticated DAST testing may be required to assess application functionality available to logged-in users.
Authentication Areas
Login workflow
Session management
Authentication requirements
User roles
Authentication persistence
Authentication configuration should be validated before executing the scan.

5️⃣ Automated DAST Scanning
Automated DAST tools interact with the running application and identify potential security vulnerabilities.
Common Testing Areas
Injection vulnerabilities
Cross-Site Scripting (XSS)
Authentication issues
Authorization-related indicators
Security misconfigurations
Security header issues
Application configuration weaknesses
Automated scanning is an important part of DAST but should be followed by manual analysis.

6️⃣ Finding Analysis
Security findings should be analyzed after the automated scan is completed.
Finding Review Process
Review the finding description
Understand the reported issue
Review the affected URL or functionality
Analyze request and response behavior
Assess the potential security impact
Determine the requirement for manual validation

7️⃣ Manual Validation
Manual validation helps confirm whether a reported finding represents a genuine security issue.
Validation Activities
Review HTTP requests and responses
Analyze application behavior
Validate security controls
Review authentication requirements
Assess exploitability
Confirm security impact
Manual validation helps improve the accuracy of security assessment results.

8️⃣ False Positive Analysis
Automated DAST tools may report findings that require additional analysis.
A finding should be reviewed based on:
Application behavior
Security controls
Authentication requirements
Authorization controls
Application configuration
Exploitability
Possible Finding Outcomes
True Positive
False Positive
Needs Further Review

9️⃣ Vulnerability Reporting
A professional DAST report should clearly communicate identified security risks.
Recommended Report Structure
Executive Summary
Assessment Scope
Assessment Methodology
Risk Rating Methodology
Vulnerability Summary
Detailed Findings
Risk Description
Business Impact
Technical Impact
Evidence
Remediation Recommendation

🔟 Remediation Tracking
After security findings are reported, remediation status should be tracked with the relevant application owners and development teams.
Remediation Activities
Share security findings
Discuss remediation recommendations
Track vulnerability status
Monitor remediation progress
Coordinate with application teams

1️⃣1️⃣ Retesting
Retesting is performed after remediation to verify whether the reported vulnerability has been addressed.
Retesting Process
Review the original finding
Understand the implemented fix
Reproduce the original test scenario
Validate the security control
Confirm the vulnerability status
Document the retest result
Possible Outcomes
Remediated
Partially Remediated
Not Remediated
Risk Accepted

🛠️ DAST & Security Testing Tools
AppScan on Cloud (ASoC)
WebInspect
Burp Suite
OWASP ZAP
Tool selection depends on the application scope, architecture and assessment requirements.

📚 Security References
OWASP Top 10
OWASP Web Security Testing Guide
OWASP Application Security Verification Standard

⚠️ Disclaimer
This repository is intended for educational and authorized application security testing purposes.
Always obtain proper authorization before performing security testing against any application or system.

👨‍💻 Author
G. Mahesh Babu
Application Security Engineer | VAPT | SAST | DAST | SCA | DevSecOps

