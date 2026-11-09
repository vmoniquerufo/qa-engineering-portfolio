Digital Banking Application - Manual Testing

1. Project Overview

This project focuses on manual testing of a fictional digital banking application.

The objective is to validate essential banking functionalities, identify potential defects, and ensure that transactions and account-related activities work as expected.

This project is created for QA portfolio demonstration purposes. All application details and test data are fictional.

2. Scope of Testing

The following functionalities are included:
* User Authentication
* Account Balance Inquiry
* Fund Transfer
* Transaction History
* Input Validation
* Error Handling

3. Test Scenarios

Scenario ID	  Test Scenario	                                                Priority
TS-001	      Verify login using valid credentials	                        High
TS-002	      Verify login using invalid credentials	                      High
TS-003	      Verify account balance display	                              High
TS-004	      Verify successful fund transfer	                              Critical
TS-005	      Verify fund transfer with insufficient balance	              Critical
TS-006	      Verify fund transfer with invalid recipient details	          High
TS-007	      Verify transaction history display	                          Medium
TS-008	      Verify transaction details after successful transfer	        High
TS-009	      Verify required field validation during fund transfer	        High
TS-010	      Verify handling of network interruption during fund transfer	Critical

4. Detailed Test Cases

TC-001: Login with Valid Credentials

Preconditions:
* User has an active banking account.
* User has valid login credentials.

Test Steps:
1. Navigate to the login page.
2. Enter a valid username.
3. Enter a valid password.
4. Click the Login button.

Expected Result:
* User is successfully authenticated.
* User is redirected to the account dashboard.
* Account information is displayed.

TC-002: Login with Invalid Credentials

Preconditions:
* User is on the login page.

Test Steps:
1. Enter a valid username.
2. Enter an incorrect password.
3. Click the Login button.

Expected Result:
* User is not authenticated.
* An appropriate error message is displayed.
* User remains on the login page.

TC-003: Fund Transfer with Insufficient Balance

Preconditions:
* User is logged in.
* Source account has insufficient available balance.

Test Steps:
1. Navigate to the Fund Transfer page.
2. Select the source account.
3. Enter valid recipient details.
4. Enter a transfer amount greater than the available balance.
5. Submit the transaction.

Expected Result:
* Transaction is rejected.
* An insufficient balance message is displayed.
* No amount is deducted from the source account.
* No transaction is recorded as successful.

5. Test Execution
Test execution will be documented separately after the test environment and application behavior have been established.

6. Test Environment

* Application: Fictional Digital Banking Application
* Testing Type: Manual Testing
* Test Level: Functional Testing
* Tools: Jira (Defect Tracking), Markdown (Documentation)
* Test Data: Dummy accounts and fictional transaction details

7. Project Notes

This is an independent QA portfolio project. Test scenarios and expected results are based on defined sample requirements and do not represent a live banking application.
