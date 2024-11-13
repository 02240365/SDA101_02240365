# Hostel Room Maintenance Form

This document describes the structure of the Hostel Room Maintenance Form.

## Form Fields

1. **Name**
   - Type: Text input
   - Required: Yes

2. **Room No**
   - Type: Dropdown
   - Options:
     - New Building 1
     - New Building 2
     - Common Mess
     - LPF
     - UPF
     - Transit
     - Executive
     - B-type

3. **Type of Issue**
   - Type: Text input

4. **Description**
   - Type: Text input

5. **Urgency**
   - Type: Dropdown
   - Required: Yes
   - Options:
     - Immediate
     - Medium
     - Low

6. **Submit Button**
   - Type: Button

## Notes

- This form is designed to collect information about maintenance issues in hostel rooms.
- The form uses CSS styling (referenced in `styling_form.css`).
- All fields should be filled out before submitting the form.
- The urgency level helps prioritize maintenance tasks.