# Indicators of Compromise (IOC) Register

## 1. Overview

This document contains the potential Indicators of Compromise identified during the investigation of a suspected phishing email.

The indicators are documented to support threat identification, investigation and incident response.

## 2. Identified Indicators

| No. | IOC Category  | Indicator                                                                             | Description                             |
| --- | ------------- | ------------------------------------------------------------------------------------- | --------------------------------------- |
| 1   | Email Address | [security-alert@micros0ft-security.com](mailto:security-alert@micros0ft-security.com) | Suspicious sender address               |
| 2   | Domain        | micros0ft-security.com                                                                | Potential Microsoft impersonation       |
| 3   | URL           | micros0ft-security.example/verify                                                     | Suspicious credential verification link |
| 4   | Email Subject | URGENT: Your Microsoft 365 Account Will Be Suspended                                  | Urgency-based social engineering        |

## 3. IOC Analysis

### 3.1 Suspicious Email Address

The sender address uses a domain resembling Microsoft's branding.

The number zero (0) replaces the letter 'o', potentially indicating an attempt to deceive the recipient.

### 3.2 Suspicious Domain

The domain micros0ft-security.com resembles Microsoft's identity and may be intended to create a false impression of legitimacy.

### 3.3 Suspicious URL

The supplied URL contains a domain resembling Microsoft's branding.

The `.example` domain is reserved for documentation and testing. It is not evidence of an operational phishing website.

### 3.4 Suspicious Email Subject

The subject creates urgency by threatening account suspension.

This is consistent with social engineering techniques designed to encourage immediate action.

## 4. Potential Threat

The indicators collectively suggest a possible phishing attempt intended to obtain user credentials.

Potential consequences include:

* Credential theft.
* Unauthorised account access.
* Account compromise.
* Exposure of organisational information.

## 5. Recommended SOC Actions

1. Preserve the suspicious email and associated evidence.
2. Investigate the sender domain using approved threat intelligence resources.
3. Examine the original email headers.
4. Assess the URL using an approved URL analysis service without directly visiting the suspicious destination.
5. Check whether other employees received similar emails.
6. Escalate validated indicators to the appropriate security team.
7. Recommend blocking confirmed malicious indicators according to organisational policy.

## 6. IOC Validation Status

| Indicator      | Validation Status                               |
| -------------- | ----------------------------------------------- |
| Sender address | Observed; authenticity not verified             |
| Sender domain  | Observed; maliciousness not confirmed           |
| Suspicious URL | Observed; live threat not established           |
| Email subject  | Observed; suspicious characteristics identified |

## 7. Conclusion

The identified indicators provide useful investigative leads for a suspected phishing incident.

However, the indicators have not all been independently validated as malicious.

Additional technical investigation is required before adding them to production security blocklists or treating them as confirmed malicious infrastructure.

**Investigation Classification:** Suspected Phishing
**Role:** SOC Analyst Level 1
