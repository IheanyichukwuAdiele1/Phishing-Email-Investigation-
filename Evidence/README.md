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
| EVD-006     | SPF authentication results      | Not yet verified  |
| EVD-007     | DKIM authentication results     | Not yet verified  |
| EVD-008     | DMARC authentication results    | Not yet verified  |
| EVD-009     | URL reputation analysis         | Not yet performed |

## 3. Evidence Sources

The initial indicators were obtained from the phishing email sample supplied for this practical investigation.

The original raw email headers and independent technical validation results were not available at the time of documentation.

## 4. Evidence Handling

The following procedures should be observed:

* Preserve original evidence without modification.
* Record the source of each evidence item.
* Avoid visiting suspicious URLs directly.
* Do not upload sensitive personal or organisational information.
* Maintain accurate records of investigation activities.
* Distinguish observed evidence from assumptions.

## 5. Outstanding Evidence Collection

The following activities remain outstanding:

1. Obtain the original email headers.
2. Examine SPF, DKIM and DMARC results.
3. Conduct safe URL reputation analysis.
4. Capture genuine screenshots of available investigation results.
5. Update the investigation report with validated findings.

## 6. Conclusion

Evidence collection and preservation are essential components of a reliable SOC investigation.

This inventory identifies the available evidence and highlights the additional technical validation required to complete the investigation.
