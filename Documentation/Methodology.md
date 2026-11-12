# Phishing Email Investigation Methodology

## 1. Introduction

This document outlines the methodology used to investigate a suspected phishing email as part of a SOC Analyst Level 1 practical exercise.

The investigation focuses on identifying suspicious email characteristics, examining potential indicators of compromise and assessing possible security risks.

## 2. Investigation Process

### Step 1: Email Content Examination

The supplied email was examined to identify suspicious language, unusual requests and possible social engineering techniques.

Particular attention was given to:

* Urgency and threats of account suspension.
* Requests to verify login credentials.
* Suspicious instructions or links.

### Step 2: Sender Analysis

The sender address and domain displayed in the supplied email sample were examined for inconsistencies and possible impersonation. No independent email-header verification was performed.

The investigation identified:

* Sender: [security-alert@micros0ft-security.com](mailto:security-alert@micros0ft-security.com)
* Domain: micros0ft-security.com

The substitution of the letter 'o' with the number '0' was identified as a possible domain impersonation technique.

### Step 3: URL Examination

The verification link supplied in the email was examined to identify possible domain impersonation.

The observed URL was:

https://micros0ft-security.example/verify

The domain resembles Microsoft's branding and requires further validation.

The `.example` domain is reserved for documentation and testing. No live malicious website was established through this exercise.

### Step 4: Email Authentication Assessment

SPF, DKIM and DMARC authentication results were identified as important evidence for validating sender authenticity.

However, the original email headers were not available.

Consequently, authentication results could not be independently verified.

### Step 5: IOC Identification

Potential Indicators of Compromise were documented, including:

* Suspicious sender address.
* Suspicious sender domain.
* Suspicious verification URL.
* Urgency-based email subject.

### Step 6: Risk Assessment

The potential consequences of interacting with the suspicious email were assessed.

These included credential theft, unauthorised account access and possible exposure of organisational information.

### Step 7: Incident Response Recommendations

Appropriate SOC Level 1 recommendations were identified.

These included preserving the email, advising the recipient not to interact with the link, reporting the incident and escalating the investigation.

## 3. Investigation Principles

The investigation followed these principles:

* Evidence-based analysis.
* Proper documentation.
* Avoidance of unsupported conclusions.
* Appropriate escalation.
* Compliance with organisational security procedures.

## 4. Conclusion

The methodology provided a structured approach to investigating a suspected phishing email.

It enabled the identification of suspicious characteristics, documentation of potential IOCs and development of appropriate incident response recommendations.

Further technical validation would be necessary to establish the full nature and impact of the suspected incident.
A separate Gmail email was also examined as an email authentication training exercise. SPF, DKIM and DMARC returned PASS. These results belong to the separate training email and must not be interpreted as authentication results for the original phishing sample.
