Digital Banking Application - Bug Reports

1. Overview

This document defines the defect reporting format for the fictional Digital Banking Application.

The purpose is to demonstrate proper defect documentation, including reproducibility, expected versus actual results, severity, and priority.

All examples in this document are illustrative and are not actual defects observed in a live application.

2. Bug Report Template

Field	Description
Bug ID - Unique defect identifier
Summary - Short description of the defect
Module - Affected application module
Environment - Environment where the defect occurs
Preconditions - Conditions required before reproduction
Steps to Reproduce - Detailed steps to reproduce the issue
Expected Result - Intended application behavior
Actual Result - Observed application behavior
Severity - Impact of the defect
Priority - Urgency of fixing the defect
Status - Current defect status

3. Sample Bug Report

BUG-001: Duplicate Transaction Record After Repeated Submission

Module: Fund Transfer
Environment: Sample Testing Environment
Severity: Critical (Illustrative)
Priority: High (Illustrative)

Preconditions:
* User is logged in.
* User has sufficient account balance.
* A valid recipient account is available.

Steps to Reproduce:
1. Navigate to the Fund Transfer page.
2. Enter valid recipient details.
3. Enter a valid transfer amount.
4. Click the Submit button.
5. Simulate a delayed response from the application.
6. Submit the transaction again, if the interface allows it.
7. Check the transaction history and account balance.

Expected Result:
* The application should prevent duplicate transaction processing.
* Only one transaction should be recorded.
* The account should only be debited once.

Actual Result:
Illustrative scenario: Two transaction records appear for the same transfer request.

Status: Example Only - Not Executed

4. Severity Classification
* Critical: Defects that may cause significant financial impact, data corruption, or major system failure.
* High: Defects affecting important application functionality.
* Medium: Defects affecting functionality with available workarounds.
* Low: Minor UI, usability, or cosmetic issues.

5. Priority Classification
* High: Requires immediate attention or resolution.
* Medium: Should be addressed within the planned development cycle.
* Low: Can be scheduled for a future release.

6. Defect Lifecycle
New → Assigned → In Progress → Fixed → Retest → Closed

If the issue persists after retesting, the defect may be reopened.

7. QA Considerations

When reporting defects, the following should be considered:
* Ensure the issue is reproducible whenever possible.
* Provide clear and concise reproduction steps.
* Include relevant screenshots, logs, or API responses when available.
* Differentiate between severity and priority.
* Verify the fix through retesting.
* Perform regression testing on affected functionalities.

8. Notes

This document is part of an independent QA portfolio project. The sample defect is hypothetical and will be validated against actual application behavior before being presented as an executed finding.
