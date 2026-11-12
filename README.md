# Phishing Email Investigation | SOC Analyst Level 1

## 1. Project Overview

This project demonstrates a practical Security Operations Centre (SOC) Analyst Level 1 investigation of a suspected phishing email.

The investigation focuses on identifying email-based threats, examining suspicious sender information, detecting domain impersonation, analysing suspicious URLs, identifying Indicators of Compromise (IOCs), and recommending appropriate incident response actions.

This is a controlled cybersecurity training exercise designed to demonstrate fundamental SOC investigation and analytical skills.

## 2. Investigation Objectives

* Identify potential phishing indicators in a suspicious email.
* Examine sender addresses and domain legitimacy.
* Identify possible brand impersonation.
* Examine suspicious URLs and domains.
* Identify and document Indicators of Compromise (IOCs).
* Assess potential risks to the organisation.
* Recommend appropriate incident response measures.

## 3. Scenario

An employee, John Doe, receives an urgent email claiming that his Microsoft 365 account will be suspended unless he verifies his login credentials.

The email contains a suspicious verification link and uses a sender domain that resembles Microsoft's legitimate domain.

The SOC Analyst is required to investigate the email and determine whether it exhibits characteristics of a phishing attempt.

## 4. Suspicious Email Indicators

| Indicator          | Observation                                                                           |
| ------------------ | ------------------------------------------------------------------------------------- |
| Sender             | [security-alert@micros0ft-security.com](mailto:security-alert@micros0ft-security.com) |
| Sender Domain      | micros0ft-security.com                                                                |
| Subject            | URGENT: Your Microsoft 365 Account Will Be Suspended                                  |
| Impersonated Brand | Microsoft                                                                             |
| Suspicious URL     | micros0ft-security.example/verify                                                     |
| Primary Concern    | Possible credential harvesting                                                        |

## 5. Investigation Methodology

The investigation covers the following areas:

1. Sender and domain analysis.
2. Email authentication assessment.
3. Identification of brand impersonation.
4. Suspicious URL examination.
5. Identification of Indicators of Compromise.
6. Threat assessment and incident classification.
7. Incident response recommendations.

## 6. Preliminary Findings

The email exhibits several characteristics associated with phishing:

* A sender domain resembling Microsoft's brand name.
* Character substitution in the domain name.
* Urgent language intended to pressure the recipient.
* A request to verify login credentials through a suspicious link.

These indicators suggest a potential credential-harvesting attempt.

Further technical validation of email authentication results and URL behaviour is required before making a complete determination.

## 7. Potential Security Risks

* Unauthorised access to corporate accounts.
* Credential theft.
* Account compromise.
* Unauthorised access to organisational information.
* Potential data exposure.

## 8. Recommended Security Actions

* Do not click the suspicious link.
* Do not submit credentials.
* Preserve the email for investigation.
* Report the email to the appropriate security team.
* Block or quarantine the message where authorised.
* Investigate whether other employees received the same email.
* Escalate confirmed or suspected compromise according to organisational procedures.

## 9. Skills Demonstrated

* Phishing email investigation.
* Email security analysis.
* Domain impersonation detection.
* IOC identification.
* Threat assessment.
* Security incident documentation.
* SOC Level 1 investigation and escalation.

## 10. Project Status
**Status: Documentation and Training Evidence Completed — Technical Validation Limited**

The phishing email investigation has been documented as part of a practical SOC Analyst Level 1 portfolio.

Completed activities include:

* Phishing email content and sender analysis.
* Identification of suspicious indicators of compromise (IOCs).
* URL structure and impersonation assessment.
* Email authentication training exercise (separate from the original phishing sample).
* Evidence inventory and investigation documentation.
* Reconstructed training screenshots.

**Investigation Limitations:**

The original raw email headers were not available. SPF, DKIM and DMARC results for the original phishing email remain unverified. The `.example` URL is reserved for training and was not subjected to live reputation analysis.

This project demonstrates practical SOC Analyst Level 1 skills in phishing analysis, evidence documentation, threat identification and incident assessment.


---

**Disclaimer:** This project is conducted for educational and cybersecurity training purposes. Suspicious indicators are documented for analysis and do not independently establish that a domain or email has been technically verified as malicious.
