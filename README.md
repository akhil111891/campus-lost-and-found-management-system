# Campus Lost & Found Management System with AI Matching

A ServiceNow application designed to simplify campus lost and found management through centralized reporting and automated item matching.

## About the Project

The Campus Lost & Found Management System is developed to address a common problem faced by college students: finding lost belongings and connecting them with the students who reported them missing.

The application provides a centralized platform where students can report lost and found items. An automated matching engine compares submitted reports and identifies possible matches based on item attributes.

Students can review relevant match suggestions, examine found item details, and confirm ownership through the application.

## Project Demonstration

Watch the complete demonstration of the application, including student reporting, automated matching, match suggestions, and ownership confirmation.

🎥 **[Watch Project Demonstration](https://drive.google.com/file/d/1cMEJ-G9HBV6tPJ9j4IHyJaDjw67IBAMY/view?usp=drive_link)**

## Features

- **Lost Item Reporting:** Allows students to report lost belongings by providing item details such as name, category, brand, colour, description, location, and date.
- **Found Item Reporting:** Enables students to report items they have found on campus with relevant details and photographs.
- **Automated Item Matching:** Compares lost and found reports using multiple attributes to identify possible matches.
- **Match Scoring:** Calculates matching scores based on category, brand, colour, description, location, and date.
- **Relevant Match Suggestions:** Displays qualifying suggestions to the student associated with the corresponding lost item report.
- **Found Item Details:** Allows students to examine suggested found item information before confirming ownership.
- **Ownership Confirmation:** Provides an option for students to indicate that a suggested found item belongs to them.
- **Report Tracking:** Allows students to view and track their submitted lost and found reports.

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

1. A student submits a lost item report through the application.
2. Another student submits a found item report.
3. The application automatically triggers the matching process when a report is submitted.
4. The matching engine compares the attributes of the lost and found items.
5. A matching score is calculated using the configured comparison criteria.
6. Only matching scores strictly greater than 75 qualify for suggestions.
7. A match suggestion is created for the corresponding lost item report.
8. The student who reported the lost item can view the relevant suggestion.
9. The student reviews the found item details and can confirm ownership.
10. The application updates the relevant claim and report information according to the configured workflow.

## Matching Engine

The matching engine evaluates six attributes to calculate the matching score.

| Attribute | Weight |
|---|---:|
| Category | 25 |
| Brand | 20 |
| Colour | 15 |
| Description | 20 |
| Location | 10 |
| Date | 10 |
| **Total** | **100** |

### Matching Conditions

- Only scores strictly greater than 75 qualify for match suggestions.
- The found date must be on or after the lost date.
- The found date must be within seven days of the lost date.

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

[Campus Lost & Found Management System](https://dev295777.service-now.com/campus_lost_found)

A demonstration account is available for exploring the application. Please contact the project developer for access details.

## Project Screenshots

Selected screenshots demonstrate the application's interface, data structure, matching logic, and workflow.

## Testing

The following scenarios can be used to verify the application workflow:

1. Submit a new lost item report.
2. Submit an unrelated found item report.
3. Verify that an unrelated item does not generate an irrelevant suggestion.
4. Submit a found item report matching an existing lost report.
5. Verify the matching score and generated suggestion.
6. Review the found item details.
7. Test the ownership confirmation process.
8. Verify the relevant report and suggestion status updates.

## Future Improvements

- Improve matching accuracy using advanced matching techniques.
- Introduce additional student notifications.
- Enhance reporting and tracking capabilities.
- Improve application security and data access controls.
- Expand testing for different matching and ownership scenarios.

---

**Project:** Campus Lost & Found Management System with AI Matching

**Platform:** ServiceNow

**Purpose:** Simplifying campus lost and found management through automated item matching.
