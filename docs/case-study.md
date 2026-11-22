# Universal Business CRM & Alert Automation

## Professional Project Case Study

**Project:** Automated CRM, Lead Management & Business Monitoring System  
**Developer:** Ebiowei Peter  
**Role:** n8n Workflow Automation Developer  
**Project Type:** Independent Portfolio Project  
**Date:** November 2026  
**Technologies:** n8n, JavaScript, Google Sheets, JSON, n8n Data Tables and GitHub

---

## 1. Project Overview

I developed a Universal Business CRM & Alert Automation system to demonstrate how businesses can organize customer enquiries, reduce duplicate records, prioritize leads, prepare follow-ups and monitor automation workflows.

The project uses n8n to connect customer data processing, CRM integration, conditional routing, error handling and operational monitoring.

The original development workflow contains 98 nodes and 75 connection entries.

This is an independent portfolio project tested using controlled datasets rather than a live client production deployment.

## 2. Business Problem

Businesses that manage customer enquiries manually can experience several operational challenges:

- Incomplete or inconsistent customer information
- Duplicate CRM records
- Difficulty identifying high-priority enquiries
- Delayed or forgotten customer follow-ups
- Repetitive administrative work
- Limited visibility into workflow errors
- Difficulty tracking operational alerts

These problems can make customer management less organized and increase the amount of manual checking required.

## 3. Proposed Solution

I designed an n8n automation workflow that processes customer enquiries through several connected modules.

The system demonstrates how to:

1. Validate incoming customer information.
2. Retrieve existing CRM records.
3. Detect duplicate customer entries.
4. Classify enquiries by business type.
5. Assign lead priorities.
6. Identify follow-up requirements.
7. Prepare follow-up messages.
8. Detect processing errors and repeated events.
9. Track alert history.
10. Generate operational monitoring reports.

## 4. Technical Implementation

### Customer Data Validation

JavaScript validation rules check customer information before further processing.

The workflow identifies incomplete or invalid records and prevents them from proceeding through normal processing routes without review.

### Google Sheets CRM Integration

The workflow retrieves existing customer records from Google Sheets.

A composite customer identifier combines the business name and email address after normalization.

This allows the workflow to detect repeated customer entries within the same business while distinguishing records belonging to different businesses.

### Business Classification and Routing

Conditional logic classifies supported enquiries and directs them through relevant workflow branches.

Unsupported or unclear classifications can be directed to manual review.

### Lead Priority Scoring

Predefined rules assign lead priorities such as High, Medium and Low.

This provides a structured way to identify enquiries that may require earlier attention.

### Follow-Up Management

The workflow evaluates follow-up requirements and classifies tasks as:

- Overdue
- Due Today
- Scheduled
- Not Required

It also prepares follow-up messages for review. Automatic message delivery was not part of the verified final demonstration.

### Error Handling and Replay Protection

The project includes controlled tests for processing failures, retry limits, duplicate events and manual-review conditions.

These mechanisms demonstrate how workflows can identify problems and reduce the risk of repeated operations.

### Persistent Alert History

n8n Data Tables store test alert-history records.

The workflow includes replay checks, alert-state validation and operational monitoring logic.

### Monitoring and Reporting

Monitoring modules summarize alert states, identify unresolved records and generate reports for operational review.

## 5. Testing and Verification

The project was tested using controlled datasets and simulated workflow events.

Verified development results include:

| Verification Area | Result |
|---|---|
| Original development workflow | 98 nodes |
| Connection entries | 75 |
| Final edge-case tests | 5 of 5 passed |
| Broken connection references | 0 |
| Baseline Google Sheets CRM records | 5 |
| Persistent alert-history test records | 3 |
| CRM writes during final audit | 0 |
| Notifications sent during final audit | 0 |

The final checks confirmed that the tested workflow structure remained intact and that the restricted write and notification operations were not executed.

## 6. Technical Challenges and Lessons

The project provided practical experience in:

- Designing connected n8n workflows
- Writing JavaScript validation and transformation logic
- Integrating Google Sheets with automation processes
- Preventing duplicate customer records
- Handling conditional routing
- Implementing retry limits and event replay checks
- Managing persistent alert-history data
- Testing edge cases
- Documenting workflows for review and maintenance

The project also reinforced the importance of testing changes before enabling operations that modify external records.

## 7. Potential Business Benefits

A suitably configured automation system could help businesses:

- Reduce repetitive customer data processing
- Improve CRM record consistency
- Organize enquiries by priority
- Track pending follow-ups
- Identify workflow failures earlier
- Improve visibility into operational processes

These are potential benefits. The project did not measure actual time savings, revenue improvements or client business outcomes.

## 8. Project Limitations

The workflow was developed and tested as a portfolio demonstration.

It has not been verified as a live production deployment.

The final audit did not include actual CRM write operations or notification delivery.

Some historical audit warnings remained unresolved, and the stored alert records had incomplete severity information.

The duplicate and replay protection tests do not establish concurrency-safe processing under production workloads.

Additional testing, security review, operational configuration and client-specific requirements would be necessary before production deployment.

## 9. Conclusion

The Universal Business CRM & Alert Automation project demonstrates practical experience in n8n workflow development, JavaScript, CRM integration, lead management, error handling and operational reporting.

It provides a documented example of my ability to design, connect, test and explain business automation workflows.

I am interested in applying these skills to freelance projects involving CRM automation, Google Sheets integration, customer enquiry processing and business process automation.

## 10. Project Repository

**GitHub:** https://github.com/EbioweiPeter/n8n-universal-business-automation

**Developer:** Ebiowei Peter  
**Specialization:** n8n Workflow Automation and CRM Integration
