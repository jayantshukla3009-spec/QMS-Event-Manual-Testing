Event (Deviation) Module – Manual Test Cases
Overview
This repository contains manual test cases for the Event (Deviation) module of a Quality Management System (QMS). The test cases were written based on exploratory testing of the application and cover end-to-end functional, UI, and negative scenarios across all major sections of the Event page.

Module Under Test
Application: QMS – Event (Deviation) Module
Page: Event Creation & Management Page
Testing Type: Manual / Black-Box Testing

Objective
To validate the functionality, usability, and data integrity of the Event (Deviation) module — ensuring all form fields, workflow navigation, validations, and UI components behave as expected.

Test Scope
In Scope

Event creation and form field validations
Mandatory field checks and Save Draft behavior
Workflow navigation and stage handling
UI and field-level validations
AI Agent / AI Co-Pilot panel interaction
Error messages and system responses
Sidebar navigation (Event Details, History Log, Team Chat, Deadlines)
Affected Items management (add, edit, delete)
File upload behavior and system messaging

Out of Scope

Login and authentication functionality
Other QMS modules (CAPA, Complaints, Recall, etc.)
Backend and database-level validation
Performance and load testing


Test Artifacts
ArtifactDescriptionEvent_Deviation_Test_Cases.xlsx100 manual test cases across 10 modulesREADME.mdThis file – test scope and documentation

Test Case Coverage
ModuleTest CasesA. Header & Top BarTC_001 – TC_015B. Event Workflow Navigation BarTC_016 – TC_022C. Sidebar NavigationTC_023 – TC_038D. Event Basics – Form FieldsTC_039 – TC_057E. Product Impact AssessmentTC_058 – TC_060F. Scope & ContextTC_061 – TC_072G. Quick Scope BoundaryTC_073 – TC_076H. Additional DetailsTC_077 – TC_087I. Save / Save Draft / OptionsTC_088 – TC_095J. UI Confirmation After Save DraftTC_096 – TC_097K. Intermittent IssuesTC_098 – TC_100

Test Design Techniques Used

Equivalence Partitioning – valid and invalid input classes
Boundary Value Analysis – field limits and edge cases
Negative Testing – missing mandatory fields, empty states, locked stages
UI Testing – layout, alignment, labels, indicators
Exploratory Testing – session-based testing of AI Co-Pilot, workflow, and intermittent bugs


Test Case Structure
Each test case includes the following fields:
FieldDescriptionModuleFunctional area being testedTC_IDUnique test case identifierScenarioWhat is being testedTest TypePositive / Negative / UI / FunctionalTest StepsStep-by-step actionsTest DataInput data usedExpected ResultWhat should happenActual ResultWhat actually happenedStatusPASS / FAIL

Bugs / Failures Identified
Key failures found during testing:

Notification icon is non-interactive (TC_005)
My Profile dropdown is non-interactive (TC_008)
AI Co-Pilot Refresh button navigates to blank screen (TC_012)
Mic and Attachment icons in AI panel are non-interactive (TC_014, TC_015)
Mandatory dropdown, Date & Time, and Detected By fields allow Save Draft without validation (TC_045, TC_047, TC_052)
Radio button gets deselected on re-click — incorrect behavior (TC_076)
Mandatory text fields allow Save Draft without validation (TC_079)
Bullet points / numbered list formatting not working (TC_081)
File upload UI is inconsistent with 'not implemented' message (TC_085–TC_087)
Team Chat and Deadlines sidebar sections render blank page (TC_098, TC_099)


Author
Jayant Kumar Shukla
QA Automation Engineer
LinkedIn | GitHub