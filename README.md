# Vacation Management Power Platform Solution

## Overview

This project demonstrates an end-to-end vacation management solution built using Microsoft Power Platform technologies.

The solution enables employees to submit vacation requests, managers to review and approve requests, and HR teams to monitor vacation planning across departments.

### Technologies Used

- Power Apps
- Power BI
- Power Automate
- SharePoint Online
- DAX

---

## Business Problem

Managing vacation requests through emails and spreadsheets often creates:

- Lack of visibility for managers
- Manual approval processes
- Delayed communication
- Difficulty tracking vacation patterns
- Limited workforce planning capabilities

This solution centralizes the entire process into a single digital workflow, improving transparency, efficiency, and workforce planning.

---

## Solution Architecture

```text
Employees
    ↓
Power App
    ↓
SharePoint Lists
    ↓
Power BI Dashboard

Power Automate
    ↓
Notifications & Approvals

HR & Managers
```

---

## Main Features

### Employee Experience

- Submit vacation requests
- Edit existing requests
- View request status
- Access from web, mobile, and tablet

### Manager Experience

- Review requests
- Approve or reject requests
- Track team availability

### HR Experience

- Access all requests
- Monitor approval status
- Support workforce planning

---

## Power Automate Workflows

### Employee Notifications

Automatic notifications when a request is:

- Approved
- Rejected

### Manager Notifications

Automatic notifications when:

- A new request is submitted
- Vacation start dates are approaching (two-week reminder)

### HR Notifications

Automatic notifications when managers update the status of a request.

### Future Enhancements

- Monthly department summaries
- Workforce planning alerts
- Capacity monitoring reports

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

Master employee information repository containing:

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

---

## Business Value Delivered

This solution provides:

- Centralized vacation management
- Improved approval process visibility
- Reduced manual administrative work
- Better workforce planning capabilities
- Real-time reporting and monitoring
- Enhanced communication across stakeholders

---

## Project Status

**Portfolio Project / Case Study**

This project was developed to demonstrate how Microsoft Power Platform can be used to automate HR processes, streamline vacation management, and provide actionable business insights through analytics.
