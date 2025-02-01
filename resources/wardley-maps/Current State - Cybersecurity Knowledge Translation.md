# Current State - Cybersecurity Knowledge Translation

In this Wardley map, we can see the current state of Cybersecurity Knowledge Translation in organisations. 

The map highlights the significant gaps and challenges in translating technical cybersecurity concepts into business understanding and decision-making processes. 

The map reveals several key components and their relationships, from technical tools at the commodity end to the genesis-stage challenges of Cybersecurity Knowledge and Manual Translation. 

It particularly emphasises how security knowledge flows (or struggles to flow) from technical teams to board-level decision makers.

```wardleymap


anchor Board Members [0.95, 0.32]


component Cyber Security Knowledge [0.91, 0.11] label [-32.04, 14.34]
component Security Decisions [0.84, 0.22] label [3.94, -10.00]
component Board Reports [0.76, 0.32]
component Risk Assessments [0.56, 0.32] label [-25.68, -37.52]

component Security Metrics [0.39, 0.38] label [5.00, -0.48]
component Technical Analysis [0.25, 0.31] label [-34.15, 6.93]
component Manual Translation [0.58, 0.15] label [-56.38, -36.46]
component PowerPoint Decks [0.70, 0.51] label [5.00, -18.47]

component Security Tools [0.12, 0.53]
component Threat Intel [0.04, 0.72]

component Email [0.42, 0.73]

component Compliance Requirements [0.36, 0.67] label [-43.68, 10.11]
component Audit Reports [0.43, 0.47]
component Security Budgets [0.73, 0.18] label [-60.61, -16.35]

component CISO Business Knowledge [0.38, 0.11] label [-37.33, 11.16]
component Cyber Security Language [0.35, 0.22] label [-30.98, 12.22]
component Security Tooling [0.05, 0.48] label [-64.84, -14.23]

Cyber Security Knowledge->Security Decisions

CISO->Board Reports
Security Decisions->Board Reports

Risk Assessments->Security Metrics
Security Metrics->Manual Translation

Technical Analysis->Security Tools
Security Tools->Threat Intel
Board Reports->PowerPoint Decks
Board Reports->Email


Compliance Requirements->Audit Reports
Audit Reports->Security Metrics
Security Budgets->Security Decisions


Tech-to-Business Gap->Manual Translation
CISO Business Knowledge->Manual Translation
Cyber Security Language->Manual Translation



Board Members->Business Understanding
Manual Translation->Risk Assessments
Technical Analysis->Security Metrics
Cyber Security Knowledge->Board Members
Board Members->Cyber Security Knowledge
Manual Translation->Board Reports
Audit Reports->Risk Assessments

Security Tooling->Security Tools

evolution Genesis->Custom-built->Product->Commodity


size [750,600]

```


