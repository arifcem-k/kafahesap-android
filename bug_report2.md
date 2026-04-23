# Bug Report

## Title
Text overflow issue on "Geçmiş" page causes partial visibility of card data

## Description
On the "Geçmiş" page, long text values inside cards are not fully visible due to layout constraints. The content overflows the container and is neither wrapped nor scrollable, resulting in data loss from user perspective.

## Steps to Reproduce
1. Open the application  
2. Navigate to the "Geçmiş" page  
3. Ensure records with longer text values exist  
4. Observe the displayed card content  

## Expected Result
All text content should be fully visible within the card.  
Text should wrap properly or the container should support scrolling.

## Actual Result
Some parts of the text are cut off and not visible due to overflow handling issues.

## Severity
Medium

## Priority
Medium

## Notes
UI layout constraints may be too restrictive or missing proper text wrapping / overflow handling (e.g., ellipsis, scroll, or flex adjustments).
