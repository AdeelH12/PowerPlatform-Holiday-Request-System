# Employee Holiday Request & Approval System

A business application built using Microsoft Power Apps, Microsoft Dataverse and Power Automate to manage employee holiday requests and automate the approval process.

## Overview

This project allows employees to submit holiday requests through a Power Apps application. Requests are stored in Microsoft Dataverse and automatically processed through a Power Automate approval workflow.

The workflow sends the request for approval, updates the request status based on the approval outcome and sends an email notification to the employee.

## Technologies

- Microsoft Power Apps
- Microsoft Dataverse
- Microsoft Power Automate
- Microsoft Outlook
- Microsoft 365

## How It Works

1. An employee submits a holiday request through the Power Apps application.
2. The request is stored as a record in Dataverse.
3. Power Automate detects the new request.
4. An approval request is sent to the designated approver.
5. The approver chooses Approve or Reject.
6. The Dataverse record is updated with the outcome.
7. An email notification is sent to the employee.

## Workflow

```text
Power Apps
    ↓
Dataverse
    ↓
Power Automate
    ↓
Approval
   ↙ ↘
Approved  Rejected
   ↓         ↓
Update Dataverse
   ↓
Email Notification
