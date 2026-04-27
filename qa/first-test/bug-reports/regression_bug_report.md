
#Bug Report

Title
#Validation messages are truncated in alert dialog when multiple errors are displayed on Bilgiler page

Description
After fixing the validation logic to display multiple error messages simultaneously, a new issue appeared during regression testing. When multiple validation errors are shown inside the alert dialog, the message content exceeds the available UI space and gets truncated. As a result, users cannot see all validation messages بالكامل.

Steps to Reproduce

Open the application
Navigate to the "Bilgiler" page
Enter invalid value (e.g., 0) for Salary field
Enter invalid value (e.g., 0) for Working Hours field
(Optional) Leave another field invalid to increase error count
Click on "Kaydet" button

Expected Result
All validation error messages should be fully visible and readable داخل الـ alert dialog (either via proper wrapping, scrolling, or expanded layout).

Actual Result
Validation messages are displayed but truncated due to limited alert dialog size. Some parts of the error text are not visible to the user.

Severity
Medium

Priority
High

Environment

Platform: Android
Build: (sen buraya version yaz → örn: v1.0.1)

Notes

This issue appeared after fixing the original validation aggregation bug.
Root cause is likely related to UI constraints of the AlertDialog component
