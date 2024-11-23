
# Garage Management Salesforce Project

## Overview

This repository documents the creation of a Garage Management system using Salesforce. The project includes features like record creation, flows, reports, dashboards, and user adoption processes. It provides an end-to-end solution for managing customer details, service appointments, billing, and feedback within a garage management system.

Each milestone represents a significant step in the implementation of the system, and the activities listed under each milestone describe the tasks that were completed during development.

---

## Table of Contents

- [Milestone 13: Flows](#milestone-13-flows)
  - [Activity 1: Create a Flow](#activity-1-create-a-flow)
  - [Activity 2: Create Another Flow](#activity-2-create-another-flow)
- [Milestone 14: Apex Trigger](#milestone-14-apex-trigger)
  - [Activity 1: Apex Handler](#activity-1-apex-handler)
  - [Trigger Handler](#trigger-handler)
- [Milestone 15: User Adoption](#milestone-15-user-adoption)
  - [Activity 1: Creating Records](#activity-1-creating-records)
- [Milestone 16: Reports](#milestone-16-reports)
  - [Activity 1: Create a Report Folder](#activity-1-create-a-report-folder)
  - [Activity 2: Sharing a Report Folder](#activity-2-sharing-a-report-folder)
  - [Activity 3: Create a Report Type](#activity-3-create-a-report-type)
  - [Activity 4: Create a Report](#activity-4-create-a-report)
- [Milestone 17: Dashboards](#milestone-17-dashboards)
  - [Activity 1: Create Dashboard Folder](#activity-1-create-dashboard-folder)
  - [Activity 2: Create Dashboard](#activity-2-create-dashboard)

---

## Milestone 13: Flows

### Activity 1: Create a Flow
- Created a Record-triggered Flow for the Billing Details and Feedback object.
- The flow updates the Payment_Paid__c field when the Payment_Status__c field is set to "Completed".
- Added an email alert to notify customers about their payment.
  
### Activity 2: Create Another Flow
- Developed a second flow that updates the Service_Status__c field in the Service Records object to "Completed" when the Quality_Check_Status__c field is set to True.

---

## Milestone 14: Apex Trigger

### Activity 1: Apex Handler
- Created the AmountDistributionHandler class to distribute the service amount based on the selected services for a customer's vehicle appointment.

### Trigger Handler
- Developed the AmountDistribution trigger on the Appointment__c object to invoke the AmountDistributionHandler class on before insert and update events.

---

## Milestone 15: User Adoption

### Activity 1: Creating Records
- Created records for Consumer Details, Appointment, and Service Records objects.
- Ensured proper validation and service amount calculations during the record creation process.

---

## Milestone 16: Reports

### Activity 1: Create a Report Folder
- Created a report folder named "Garage Management Folder" for organizing reports.

### Activity 2: Sharing a Report Folder
- Shared the "Garage Management Folder" with the "Manager" role and granted "View" access.

### Activity 3: Create a Report Type
- Created a custom report type called "Service Information" linking Customer Details, Appointment, Service Records, and Billing Details and Feedback.

### Activity 4: Create a Report
- Created a report showing service information including customer name, appointment date, service status, and payment details.
- Added a line chart for better visualization of payment status.
- Saved the report in the "Garage Management Folder".

---

## Milestone 17: Dashboards

### Activity 1: Create Dashboard Folder
- Created a dashboard folder named "Service Rating Dashboard".
- Set up sharing settings for the folder to ensure proper access.

### Activity 2: Create Dashboard
- Created a dashboard using the "Service Information" report.
- Added a line chart component to visualize data and customized the theme.
- Subscribed to the dashboard for weekly email notifications on Mondays.

---

## How to Use

1. *Clone the repository:*
   Clone this repository to your local machine using the following command:
   ```bash
   git clone https://github.com/yourusername/garage-management-salesforce.git