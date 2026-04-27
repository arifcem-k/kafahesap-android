# Bug Report

## Title
Multiple validation error messages are not displayed simultaneously on Bilgiler page

## Description
When multiple required fields are filled with invalid values, the system displays only one validation message instead of showing all relevant error messages. This prevents the user from identifying all input issues at once.

## Steps to Reproduce
1. Open the application  
2. Navigate to the "Bilgiler" page  
3. Enter invalid value (0) for Salary field  
4. Enter invalid value (0) for Working Hours field
5. Enter invalid value (0) for Salary field
6. Click on "Kaydet" button  

## Expected Result
All validation errors for the affected fields should be displayed simultaneously.

## Actual Result
Only a single validation message is displayed, while other invalid fields are not reported.

## Severity
Medium

## Priority
High

## Notes
The issue may be related to validation flow logic where errors are processed sequentially instead of aggregated before rendering.
