# Automated CRM, Lead Management & Business Monitoring System

## Professional Project Case Study

**Developer:** Ebiowei Peter  
**Role:** n8n Workflow Automation Developer  
**Project Type:** Independent Portfolio Project  
**Date:** November 2026  
**Project Status:** Tested Development Demonstration

## 1. Business Problem

Businesses that manage customer enquiries manually across spreadsheets, emails and departments can experience several operational challenges:

- Duplicate customer records.
- Incomplete or inconsistent customer information.
- Delayed responses to high-priority enquiries.
- Missed customer follow-ups.
- Incorrect assignment of service requests.
- Limited visibility into operational failures.
- Repeated processing of customer events.

These challenges create unnecessary administrative work and make it difficult for teams to manage customer relationships consistently.

## 2. Project Objective

I designed and developed a modular business automation system using n8n to demonstrate how customer enquiry management, CRM operations, follow-up scheduling and operational monitoring can be automated with appropriate validation and safety controls.

The system was designed to support multiple business categories while allowing business-specific processing rules.

## 3. Proposed Solution

The project combines customer data processing, CRM integration, lead management and operational monitoring into a collection of connected automation modules and standalone testing branches.

The solution demonstrates:

- Customer enquiry validation and normalization.
- Google Sheets CRM integration.
- Composite-key customer deduplication.
- Business classification and conditional routing.
- Lead priority scoring and department assignment.
- Follow-up scheduling and message preparation.
- Customer response and event tracking.
- Controlled CRM update simulation.
- Failure detection and retry handling.
- Persistent alert history.
- Duplicate event and replay protection.
- Alert escalation and operational reporting.

## 4. Technical Implementation

The system was developed using the following technologies:

| Technology | Application |
|---|---|
| n8n | Workflow design and orchestration |
| JavaScript | Custom business logic and data validation |
| Google Sheets | Customer relationship management |
| n8n Data Tables | Persistent alert history |
| JSON | Structured data processing and workflow portability |
| GitHub | Project documentation and version control |

### Customer Data Management

Customer records are validated, normalized and compared against existing CRM records using a composite key based on the business name and customer email address.

This design helps identify duplicate records within the same business without incorrectly rejecting enquiries associated with different businesses.

### Lead Management and Follow-Up

The workflow uses rule-based scoring to classify supported customer enquiries into high, medium and low priorities.

Follow-up tasks are scheduled according to priority, while unsupported records are routed for manual review. Customer messages are prepared without automatic delivery.

### Reliability and Operational Monitoring

The project includes event validation, duplicate protection, retry limits, audit logging, persistent alert history and escalation decisions.

Operational reports summarize alert states and identify records requiring attention.

## 5. Supported Business Applications

The business classification module supports:

- Solar energy businesses.
- Real estate companies.
- E-commerce businesses.
- Digital agencies.
- Electronics businesses.
- Digital marketing businesses.

Dedicated priority scoring rules were developed for solar energy and real estate enquiries.

The underlying automation design can be adapted to other industries according to their individual business requirements.

## 6. Verified Development Results

The original development workflow was evaluated using controlled training datasets.

| Verification | Recorded Result |
|---|---:|
| Workflow nodes | 98 |
| Connection entries | 75 |
| Baseline CRM records | 5 |
| Persistent alert history records | 3 |
| Day 25 edge-case tests | 5 of 5 passed |
| Replay attempts blocked in Day 22 testing | 3 |
| Broken connection references | 0 |
| Duplicate node names | 0 |
| CRM writes during final audit | 0 |
| Notifications sent during final audit | 0 |

Tests demonstrated customer deduplication, conditional routing, priority scoring, follow-up scheduling, retry handling, replay detection and operational reporting under controlled development conditions.

## 7. Potential Business Benefits

The automation design can help businesses:

- Reduce repetitive customer data processing.
- Improve customer record consistency.
- Identify high-priority enquiries earlier.
- Organize customer follow-up activities.
- Route service requests to appropriate teams.
- Reduce the risk of repeated event processing.
- Improve visibility into workflow failures.
- Maintain traceable records of operational activities.

These are intended benefits of the automation design, not measured outcomes from a live client deployment.

## 8. Safety and Data Protection

The project was developed with controlled execution and data protection in mind.

CRM update authorization was restricted during final testing. Notification delivery was simulated rather than executed.

The publicly available workflow was sanitized to remove original private credential references and storage configuration. Users must configure their own integrations before testing.

## 9. Current Limitations

This project is an independent development and portfolio demonstration, not a production deployment.

- Live CRM updates and notification delivery require further verification.
- Sixteen historical audit warnings remain unresolved.
- Three persistent alert records require severity classification.
- Some validation logic depends on controlled training datasets.
- Atomic duplicate protection under concurrent execution has not been established.
- The sanitized workflow requires separate import and integration testing.

Production deployment would require additional configuration, security review and end-to-end testing.

## 10. Future Development Opportunities

The system could be extended through:

- Webhook and online form integration.
- AI-assisted customer enquiry classification.
- Email and messaging integrations.
- Database-backed CRM storage.
- Improved concurrent event processing.
- Scheduled operational reporting.
- Production monitoring and deployment.

## 11. Conclusion

This project demonstrates my practical ability to design, develop, integrate, test and document business automation workflows using n8n and JavaScript.

It provides a foundation for developing customized CRM automation, lead management, customer follow-up and operational monitoring solutions for businesses.

## Project Resources

- [GitHub Repository](https://github.com/EbioweiPeter/n8n-universal-business-automation)
- [Main Project Documentation](../README.md)
- [System Architecture](architecture.md)
- [Testing and Validation Report](../tests/test-report.md)
- [Sanitized n8n Workflow](../workflow/universal-business-crm-sanitized.json)

## Author

Ebiowei Peter

n8n Workflow Automation | CRM Automation | JavaScript | Business Process Automation

Open to freelance workflow development, business automation and system integration opportunities.