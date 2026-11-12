# Evidence Inventory – Phishing Email Investigation

## 1. Purpose

This document records the evidence identified and required during the investigation of a suspected phishing email.

It establishes an organised record of available evidence, outstanding technical validation and investigation limitations.

## 2. Evidence Register

| Evidence ID | Evidence Description            | Status            |
| ----------- | ------------------------------- | ----------------- |
| EVD-001     | Suspicious sender email address | Identified        |
| EVD-002     | Suspicious sender domain        | Identified        |
| EVD-003     | Suspicious email subject        | Identified        |
| EVD-004     | Suspicious verification URL     | Identified        |
| EVD-005     | Original email headers          | Not yet obtained  |
| EVD-006     | SPF authentication results   | Not verified for original phishing email; PASS in separate training exercise |
| EVD-007     | DKIM authentication results  | Not verified for original phishing email; PASS in separate training exercise |
| EVD-008     | DMARC authentication results | Not verified for original phishing email; PASS in separate training exercise |
| EVD-009     | URL reputation analysis      | Not performed; simulated `.example` domain |                             
| EVD-010     | Reconstructed phishing email screenshots | Captured and uploaded; training reconstruction, not original email 
| EVD-011     | Email authentication training screenshot | Captured and uploaded; separate training email, not original phishing email |
| EVD-012     | URL investigation screenshot | Captured and uploaded; reconstructed analytical evidence |


## 3. Evidence Sources

The initial indicators were obtained from the phishing email sample supplied for this practical investigation.
The original raw email headers and independent technical validation results were not available at the time of documentation.

A separate Gmail training email was examined using the Show Original feature. SPF, DKIM and DMARC returned PASS. These results are not associated with the original phishing email.
A reconstructed URL investigation screenshot was created to document the suspicious URL, its structural indicators and investigation limitations. No live website was accessed.

## 4. Evidence Handling

The following procedures should be observed:

* Preserve original evidence without modification.
* Record the source of each evidence item.
* Avoid visiting suspicious URLs directly.
* Do not upload sensitive personal or organisational information.
* Maintain accurate records of investigation activities.
* Distinguish observed evidence from assumptions.

## 5. Outstanding Evidence Collection

The following activities remain outstanding or depend on obtaining additional original evidence:

1. Obtain the original phishing email headers, if available.
2. Verify SPF, DKIM and DMARC results for the original phishing email if the original headers become available.
3. Conduct safe URL reputation analysis if a real, operational URL becomes available. Live reputation analysis was not applicable to the simulated `.example` domain.
4. Capture additional screenshots of original technical validation results if they become available.
5. Update the investigation report if new, independently validated findings emerge.


## 6. Conclusion

Evidence collection and preservation are essential components of a reliable SOC investigation.

This inventory identifies the available evidence and highlights the additional technical validation required to complete the investigation.
