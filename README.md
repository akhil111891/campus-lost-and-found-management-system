# Campus Lost & Found Management System with AI Matching

## About the Project

The Campus Lost & Found Management System is a ServiceNow application developed to simplify how students report, find, and recover lost belongings within a college campus.

The application provides a centralized platform where students can submit lost and found item reports. An automated matching engine compares the submitted information and identifies possible matches between lost and found items.

Students who report lost items can view relevant match suggestions, examine found item details, and confirm ownership through the application.

## Features

- **Lost Item Reporting:** Allows students to report lost belongings with relevant item details.
- **Found Item Reporting:** Enables students to report items they have found on campus.
- **Automated Item Matching:** Compares lost and found reports using multiple attributes.
- **Match Scoring:** Calculates matching scores based on category, brand, colour, description, location, and date.
- **Relevant Match Suggestions:** Displays qualifying suggestions to the student associated with the lost item report.
- **Found Item Details:** Allows students to examine suggested found items before confirming ownership.
- **Ownership Confirmation:** Provides an option to confirm whether a suggested item belongs to the student.
- **Report Tracking:** Allows students to track their lost and found reports.

## Technologies Used

- ServiceNow Platform
- Service Portal
- Custom Tables
- Business Rules
- Script Includes
- GlideRecord
- JavaScript
- Automated Matching Logic

## How It Works

1. A student submits a lost item report.
2. Another student submits a found item report.
3. The application automatically triggers the matching process.
4. The matching engine compares the attributes of lost and found items.
5. A matching score is calculated using configured comparison criteria.
6. Only matching scores strictly greater than 75 qualify for suggestions.
7. A match suggestion is created for the corresponding lost item report.
8. The student who reported the lost item can view the suggestion.
9. The student reviews the found item details and can confirm ownership.
10. The application updates the relevant claim and report information according to the configured workflow.

## Matching Engine

The matching engine evaluates the following attributes:

| Attribute | Weight |
|---|---:|
| Category | 25 |
| Brand | 20 |
| Colour | 15 |
| Description | 20 |
| Location | 10 |
| Date | 10 |
| **Total** | **100** |

The configured date rule requires the found date to be on or after the lost date and within seven days.

Only scores strictly greater than 75 qualify for suggestions.

## Application Modules

- Home Page
- Report a Lost Item
- Report a Found Item
- My Lost Items
- My Found Items
- My Possible Matches
- Found Item Details
- How It Works

## Application Access

**Live Application:**  
https://dev295777.service-now.com/campus_lost_found

A demonstration account is available for exploring the application. Please contact the project developer for access details.

## Project Screenshots

Selected screenshots demonstrating the application interface, data structure, matching logic, and workflow will be included in the `screenshots/` folder.

## Project Structure

```text
campus-lost-and-found-management-system/
│
├── README.md
│
└── screenshots/
    ├── application-home.png
    ├── lost-report-table.png
    ├── found-report-table.png
    ├── match-suggestion-table.png
    ├── users.png
```

## Testing

The application can be evaluated using the following scenarios:

- Submit a new lost item report.
- Submit an unrelated found item report.
- Verify that an unrelated item does not generate an irrelevant suggestion.
- Submit a matching found item report.
- Verify the matching score and generated suggestion.
- Review the found item details.
- Test the ownership confirmation process.
- Verify the relevant report and suggestion status updates.

## Future Improvements

- Improve matching accuracy using advanced matching techniques.
- Introduce additional student notifications.
- Enhance reporting and tracking.
- Improve application security and data access controls.
- Expand testing for different matching and ownership scenarios.

---

**Project:** Campus Lost & Found Management System with AI Matching  
**Platform:** ServiceNow  
**Purpose:** Simplifying campus lost and found management through automated matching.
