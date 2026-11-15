# Skill Swap Design Docs

Requirements, design and test documentation for the **Crowdsourced Skill Swap Network**, a team project for **CSE251: Software Engineering** (Faculty of Computer Science and Engineering). The platform described in these documents lets people exchange skills without money: users offer expertise (for example coding, cooking, music or design) in exchange for learning other skills from community members.

This repository contains documents and diagrams only, with no source code. The documents call the project "documentation-only". A separate implementation of the platform is at [Rewanooo22/skill-swap-platform](https://github.com/Rewanooo22/skill-swap-platform).

## What the documents cover

- **Functional requirements FR1–FR25**, grouped into authentication and profiles, skill listing and discovery, matchmaking, session scheduling, messaging, reviews and trust score, gamification, and admin and moderation.
- **Non-functional requirements** covering performance, scalability, security, privacy and accessibility.
- **Subsystem interfaces** (`AuthService`, `ProfileService`, `MatchingService`, `SessionService`, `MessageService`, `ReviewService`, `GamificationService`, `AdminService`) and a requirements-to-API traceability matrix.
- **Use cases, test requirements and test cases** for the main flows.
- **Architecture models** at Level 0, 1 and 2, a three-layer logical architecture, subsystem decomposition, and communication and control flow.
- **Internal and external interface definitions**, class diagrams, a use-case-to-class traceability matrix, sequence diagrams and data flow diagrams.
- **Effort estimation** using Fibonacci story points (52 points in total), with a Gantt chart.
- **Ethics report** covering the principles adopted, the alternatives considered and their consequences.

## Document index

### Requirements and proposal

| File | Description |
|---|---|
| [Crowdsourced Skill Swap Network.pdf](Crowdsourced%20Skill%20Swap%20Network.pdf) | Software Requirements Specification (SRS): purpose, scope, stakeholders, product functions, constraints, non-functional requirements, use cases, UML diagram descriptions, security and privacy, future enhancements |
| [Crowdsourced Skill Swap Network.docx](Crowdsourced%20Skill%20Swap%20Network.docx) | Editable Word version of the SRS |
| [proposal software.pdf](proposal%20software.pdf) | Project proposal: core idea, functional requirements FR1–FR25, identified subsystems and interfaces, traceability matrix |
| [proposal software.docx](proposal%20software.docx) | Editable Word version of the proposal |
| [requirment report.pdf](requirment%20report.pdf) | Requirements report: the proposal content plus use cases and test cases (inputs and expected outputs) |
| [req2(1).pdf](req2%281%29.pdf) | Later requirements report: the proposal content plus test requirements (with priorities), use cases, test cases and an ethics report section |

### Testing

| File | Description |
|---|---|
| [Test_Requirements_Skill_Swap.docx](Test_Requirements_Skill_Swap.docx) | Test requirements and detailed test requirements for five use cases: authentication, profile management, search, session scheduling, and reviews/ratings |
| [Detailed_Test_Requirements_Skill_Swap.docx](Detailed_Test_Requirements_Skill_Swap.docx) | Detailed test-case tables for the same five use cases (ID, scenario, test data, expected result, actual result, pass/fail) |

### Design report and diagrams

| File | Description |
|---|---|
| [Design report/Design report.pdf](Design%20report/Design%20report.pdf) | Full compiled report (63 pages): SRS content, test requirements and cases, ethics report, and design report (architecture at Levels 0–2, interface definitions, class diagrams, traceability matrix, sequence diagrams, data flow diagrams, Fibonacci estimation and Gantt chart) |
| [Design report/2.docx](Design%20report/2.docx) | Architecture models section: design overview, high-level, layered and subsystem models, and communication and control flow |
| [Design report/Interface Definitions.docx](Design%20report/Interface%20Definitions.docx) | Internal (service) and external (third-party) interface definitions |
| [Design report/High-Level System Architecture.png](Design%20report/High-Level%20System%20Architecture.png), [Design report/High-Level System Architecture2.png](Design%20report/High-Level%20System%20Architecture2.png) | High-level (system-level) architecture diagram, two versions |
| [Design report/Layered Architecture Model.png](Design%20report/Layered%20Architecture%20Model.png), [Design report/Layered Architecture Model2.png](Design%20report/Layered%20Architecture%20Model2.png) | Three-layer logical architecture (presentation, business logic, data), two versions |
| [Design report/Business Logic Subsystem Architecture.png](Design%20report/Business%20Logic%20Subsystem%20Architecture.png) | Decomposition of the business logic layer into subsystems |
| [Design report/91cd944b-...-md.jpeg](Design%20report/91cd944b-f586-4621-80c3-19554f8f8d1d-md.jpeg) | Subsystem architecture diagram (application server, subsystems, relational database) |
| [Design report/Communication & Control Flow.png](Design%20report/Communication%20%26%20Control%20Flow.png) | Communication and control flow during a skill swap |
| [Design report/Level 0 .drawio](Design%20report/Level%200%20.drawio) | Level 0 diagram source file (diagrams.net): the system with User and Admin actors and interfaces I1–I7 |
| [Design report/Level 0 .drawio (1).png](Design%20report/Level%200%20.drawio%20%281%29.png) | Exported image of the Level 0 diagram |
| [Design report/Level 111111.png](Design%20report/Level%20111111.png) | Level 1 component diagram (web application, auth, matchmaking, feedback and trust, search, email and payment components around a controller) |
| [level 00.jpg](level%2000.jpg) | Level 0 diagram: User and Admin interactions with interfaces I1–I7 |
| [level 1.jpg](level%201.jpg) | Level 1 DFD: interfaces I1–I7 routed through the controller to management modules |
| [level 2F.png](level%202F.png) | Level 2 architecture diagram: components of each module (authentication, profile, skills, matchmaking, scheduling, feedback, reports) |
| [skill swap arch digrams.pptx](skill%20swap%20arch%20digrams.pptx) | Slide deck that explains the Level 0, Level 1 and Level 2 architecture diagrams |

## Other files

These files are in the repository but are not deliverables of this project.

| File | Description |
|---|---|
| [CSE251-Project-EthicsReport.pdf](CSE251-Project-EthicsReport.pdf) | Course assignment brief for the ethics report (questions to answer) |
| [Design report/CSE251-ProjectDesignReport.pdf](Design%20report/CSE251-ProjectDesignReport.pdf) | Course assignment brief and marking rubric for the design report |
| [Design report/CaseStudy-Mom-Village 5.pptx](Design%20report/CaseStudy-Mom-Village%205.pptx) | Sample case study ("Mom-Village System") with architecture and component diagrams; reference material, not about Skill Swap |
| EcoDrop business model: [PDF](EcoDrop_Business_Model_Youssef_Mohamed_Moharramm.pdf), [DOCX](EcoDrop_Business_Model_Youssef_Mohamed_Moharramm.docx), [filled DOCX](EcoDrop_Business_Model_Filled_Final_Youssef_Mohamed_Moharram.docx) | Business Model Canvas for "EcoDrop", a separate recycling-rewards idea that is unrelated to this project |

## Viewing

Open the PDFs in any PDF viewer. Open the `.docx` and `.pptx` files in Microsoft Office, LibreOffice or Google Docs/Slides, and the `.drawio` file in [diagrams.net](https://app.diagrams.net).

## Context

Coursework for CSE251: Software Engineering. The project was a team assignment.
