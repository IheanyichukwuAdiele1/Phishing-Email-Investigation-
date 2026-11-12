# Email Authentication Analysis

## 1. Objective

The objective of this exercise was to examine email authentication results and understand how SPF, DKIM and DMARC help assess email sender authenticity.

## 2. Sample Email Information

**Email Domain:** gmail.com

**Exercise Type:** Email Header Authentication Analysis

**Source:** A separate legitimate training email.

## 3. Authentication Results

| Authentication Mechanism | Result | Assessment                                                |
| ------------------------ | ------ | --------------------------------------------------------- |
| SPF                      | PASS   | Sending server authorised under the relevant SPF policy   |
| DKIM                     | PASS   | Cryptographic signature successfully verified             |
| DMARC                    | PASS   | DMARC authentication and alignment requirements satisfied |

## 4. Technical Interpretation

### SPF (Sender Policy Framework)

SPF verifies whether the sending IP address is authorised to send email for the relevant domain.

The observed result was PASS.

### DKIM (DomainKeys Identified Mail)

DKIM uses cryptographic signatures to verify the integrity of signed email content and authenticate the signing domain.

The observed result was PASS.

### DMARC (Domain-based Message Authentication, Reporting and Conformance)

DMARC evaluates SPF and DKIM authentication results alongside domain alignment requirements.

The observed result was PASS.

## 5. Overall Assessment

The sample email successfully passed all three authentication checks.

This indicates that the email satisfied the relevant authentication requirements.

However, authentication success does not guarantee that an email is harmless. Further examination of the sender, message content, URLs and attachments may still be necessary.

## 6. Investigation Limitations

The following information was not recorded:

* Actual sending IP address.
* Full sender address.
* Detailed SPF authentication domain.
* DKIM signing domain.
* DMARC alignment details.

The findings are therefore limited to the authentication results observed during the exercise.

## 7. SOC Analyst Learning Outcomes

This exercise demonstrated an understanding of:

* Email authentication mechanisms.
* SPF verification.
* DKIM signature validation.
* DMARC authentication and alignment.
* Email header investigation.
* Limitations of email authentication results.

## 8. Conclusion

SPF, DKIM and DMARC are important mechanisms for assessing email authenticity and reducing email spoofing.

A SOC Analyst should interpret authentication results alongside other email indicators before determining whether a message is malicious.
