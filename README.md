# Vacation Management Power Platform Solution

## Overview

This project showcases an end-to-end vacation management solution built using Microsoft Power Platform technologies.

The solution enables employees to submit vacation requests, managers to review and approve requests, and HR teams to monitor vacation planning through automated workflows and interactive dashboards.

The project combines application development, workflow automation, data modeling, and business intelligence into a single HR process management solution.

### Technologies Used

- Power Apps
- Power BI
- Power Automate
- SharePoint Online
- DAX

---

## Business Problem

Managing vacation requests through emails and spreadsheets often creates:

- Limited visibility for managers
- Manual approval processes
- Delayed communication
- Difficulty tracking vacation patterns
- Poor workforce planning capabilities
- Increased administrative effort for HR teams

This solution centralizes the entire process into a single digital workflow, improving transparency, efficiency, communication, and workforce planning.

---

## Solution Preview

### Power App – Employee Dashboard

screenshots/powerapp-home.png

Displays all vacation requests submitted by the employee, including vacation periods and requested days.

### Power App – New Vacation Request

screenshots/powerapp-new-request.png

Allows employees to submit new vacation requests directly from the application.

### Power App – Manager Approval

screenshots/powerapp-manager-approval.png

Managers can review pending requests and update their status to Approved, Pending, or Rejected.

### Power App – Approval Queue Completed

screenshots/powerapp-no-pending-requests.png

Confirmation view displayed when all pending requests have already been processed.

### Power BI Dashboard – Vacation Requests Analysis

screenshots/dashboard-page-1.png

screenshots/dashboard-page-1.1.png

### Power BI Dashboard – Approval Process Monitoring

screenshots/dashboard-page-2.png

screenshots/dashboard-page-2.1.png

---

## Solution Architecture

```text
Employees
    │
    ▼
Power App
    │
    ▼
SharePoint Lists
    │
    ▼
Power BI Dashboard

Power Automate
    │
    ▼
Notifications & Approvals

HR Teams & Managers
```

---

## Main Features

### Employee Experience

- Submit vacation requests
- View submitted requests
- Track approval status
- Access from web, tablet, and mobile devices

### Manager Experience

- Review team vacation requests
- Approve or reject requests
- Monitor team availability
- Manage pending approvals

### HR Experience

- Access all requests
- Monitor approval status
- Track vacation trends
- Support workforce planning initiatives

---

## Power Automate Workflows

### Employee Notifications

Automatic notifications when a vacation request is:

- Approved
- Rejected

### Manager Notifications

Automatic notifications when:

- A new vacation request is submitted
- Upcoming vacations require planning attention
- Vacation start dates are approaching

### HR Notifications

Automatic notifications whenever a manager updates the status of a request.

### Future Enhancements

- Monthly department summaries
- Workforce planning alerts
- Capacity monitoring reports
- Department-level vacation forecasting

---

## Power BI Dashboard

### Page 1 – Vacation Requests Analysis

#### KPIs

- Total Requests
- Total Vacation Days Requested
- Current Year Vacation Days

#### Insights

- Vacation demand trends
- Seasonal vacation patterns
- Requests by department
- Requests by role
- Requests by manager

### Page 2 – Approval Process Monitoring

#### KPIs

- Approval Rate
- Pending Rate
- Rejection Rate

#### Insights

- Approval bottlenecks
- Department comparisons
- Workload monitoring
- Process efficiency analysis

---

## Data Model

The solution uses two SharePoint data sources.

### Employees

Master employee repository containing:

- Employee
- Email
- Department
- Role
- Manager

### Vacation Requests

Operational vacation request records generated directly from the Power App.

### DimEmpleados

A supporting dimension table was created to:

- Normalize employee attributes
- Avoid relationship cardinality issues
- Establish stable one-to-many relationships
- Improve reporting performance
- Simplify DAX calculations

---

## Challenges & Solutions

### Challenge 1 – Data Model Relationships

The employee and vacation request datasets contained attributes that could generate cardinality issues within the Power BI model.

**Solution**

A supporting dimension table (**DimEmpleados**) was created to normalize employee information and establish stable one-to-many relationships.

### Challenge 2 – Process Visibility

Managers and HR teams lacked a centralized view of vacation requests and approval status.

**Solution**

Interactive Power BI dashboards were developed to track request volumes, vacation trends, approval rates, and departmental activity.

### Challenge 3 – Manual Communication

The vacation approval process required manual follow-up and repetitive email exchanges.

**Solution**

Power Automate workflows were implemented to automatically notify employees, managers, and HR stakeholders throughout the approval lifecycle.

---

## Business Value Delivered

This solution provides:

- Centralized vacation management
- Improved approval process visibility
- Reduced administrative workload
- Automated stakeholder communication
- Better workforce planning
- Real-time operational reporting
- Improved employee experience
- Reduced approval delays
- Increased process transparency
- Scalable HR process automation

---

## Technical Skills Demonstrated

- Power BI Data Modeling
- DAX Measures
- SharePoint Integration
- Power Apps Development
- Power Automate Workflows
- Business Process Automation
- HR Analytics
- Dashboard Design
- Data Visualization
- Requirements Analysis
- Data Modeling Best Practices
- Workflow Design
- Microsoft Power Platform Solution Design

---

## Key Learnings

Through this project I strengthened my skills in:

- Power BI data modeling
- DAX measure development
- Power Apps design and development
- SharePoint integration
- Power Automate workflow automation
- Business process analysis
- HR analytics and reporting
- Requirements gathering
- Solution architecture design
- End-to-end Power Platform implementation

---

## Documentation

Additional project documentation is available in:

```text
/docs/Vacation-Management-Dashboard-Analysis.pdf
```

---

## Project Status

**Portfolio Project / Case Study**

This project was developed to demonstrate how Microsoft Power Platform can be used to automate HR processes, streamline vacation management, and provide actionable business insights through analytics.

It showcases the design and implementation of a complete Power Platform solution, combining application development, workflow automation, data modeling, reporting, and business process optimization in a real-world HR use case.
