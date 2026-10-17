# Assignment 1: Project Proposal and Initial Requirements

## 4.1 Team Information

Project Title: **University Club Registration System**

Group Letter - A

Muneerah Almutairi  - 2231124933

Awrad Alshammeri - 2231147283

Haya Almutairi - 2231135665

GitHub repository URL - https://github.com/Malmutairi3055/project-proposal


**Project summary** - The University Club Registration System is a web-based platform that enables students to discover university clubs and submit membership requests, club leaders to review and manage applications, and administrators to maintain club information.


## 4.2 Problem and Users
University clubs provide students with opportunities to develop interests, build friendships, acquire leadership skills, and participate in campus activities. However, when information about clubs and membership applications is handled through separate channels, such as noticeboards, messaging groups, emails, paper forms, or spreadsheets, students may struggle to find accurate information and understand how to join. Applications may also be overlooked, duplicated, or delayed when club leaders manage requests manually.

The proposed system aims to make club information and membership registration more organized and accessible. Students will be able to browse available clubs, read their descriptions, and submit membership requests online. Club leaders will be able to review requests and record decisions, while administrators will maintain the club directory. A centralised system could reduce repetitive administrative work, improve visibility of application statuses, and make the registration process more consistent. Before development begins, the team will verify the existing process through relevant university documents or discussions with students and club representatives. No interviews or observations are claimed to have been completed at this stage.

The system will have three main actors:

**Student**: Browses club listings, views club details, submits membership requests, and checks application status.

**Club Leader**: Reviews membership requests for assigned clubs and approves or rejects applications.

**Administrator**: Creates, updates, and deactivates club listings to maintain accurate information.

## 4.3 Existing Solutions


| Existing Process or Solution | Useful Features | Limitations for Our Users | Source |
|---|---|---|---|
| Current Process | Paper forms, email, messaging groups, and spreadsheets provide simple ways to share information and collect membership requests. | Information may be scattered across multiple channels, and tracking application statuses may require manual follow-up. | Observation |
| Google Forms | Allows organizations to create online forms, collect responses, and review submissions using spreadsheets. | A basic forms-and-spreadsheet workflow does not provide the same integrated club directory and role-based membership decision process. | https://support.google.com/docs/answer/6281888 |

## 4.4 Proposed Solution and Justification
The University Club Registration System will provide a central web interface where students can browse active clubs and view relevant information, including club descriptions and membership details. Students will be able to submit membership requests and view their statuses. Club leaders will access requests for their assigned clubs and record approval or rejection decisions. Administrators will manage the club directory by creating, editing, or deactivating listings.

This system will make the registration process easier by keeping club information and membership requests in one place. Unlike using separate forms or emails, students can check their application status directly. The project is suitable for three students because it focuses on a small number of main features. We can also use existing web development tools to build a simple prototype during the semester.

## 4.5 Scope and Workflows
### Scope

| In Scope | Out of Scope |
|---|---|
| Displaying active club listings and descriptions | Native mobile application development |
| Viewing individual club information | Integration with university student information systems |
| Submitting membership requests | Payments or subscription management |
| Viewing personal membership-request statuses | Event scheduling and attendance tracking |
| Reviewing, approving, and rejecting requests | Chat and social-media integrations |
| Creating, editing, and deactivating club listings | Advanced analytics and automated external notifications |
| Basic role-based access and input validation | Production-scale deployment |

### Workflow 1: Discover a Club and Apply

| Item | Description |
|---|---|
| Main Actor | Student |
| Goal | Find a suitable club and request membership. |
| Steps | The student signs in, browses active clubs, opens a club profile, reviews its information, and submits a membership request. |
| Expected Outcome | The request is saved with a pending status and associated with the student and selected club. |

### Workflow 2: Review and Decide on a Membership Request

| Item | Description |
|---|---|
| Main Actor | Club Leader |
| Goal | Process a membership request for an assigned club. |
| Steps | The club leader signs in, views pending requests for an assigned club, reviews a request, and approves or rejects it. |
| Expected Outcome | The request status is updated, and the student can view the recorded decision. |

### Workflow 3: Maintain the Club Directory

| Item | Description |
|---|---|
| Main Actor | Administrator |
| Goal | Keep club information accurate and current. |
| Steps | The administrator signs in, creates a new club listing or selects an existing listing, updates its details, and saves the changes or deactivates the listing. |
| Expected Outcome | The directory displays the updated information, and deactivated clubs are no longer available for new membership requests. |

## 4.6 Initial Requirements

### Functional Requirements

| ID | Functional Requirement | Priority |
|---|---|---|
| FR-01 | The system shall allow users to sign in using prototype accounts and provide access according to their assigned roles. | Must |
| FR-02 | The system shall display active club listings containing each club's name, description, and membership information. | Must |
| FR-03 | The system shall allow a student to submit a membership request to an active club and prevent duplicate pending requests to the same club. | Must |
| FR-04 | The system shall allow students to view the status of their own membership requests. | Must |
| FR-05 | The system shall allow club leaders to view pending membership requests for clubs assigned to them. | Must |
| FR-06 | The system shall allow club leaders to approve or reject pending membership requests and save the resulting status. | Must |
| FR-07 | The system shall allow administrators to create, edit, and deactivate club listings. | Must |
| FR-08 | The system shall validate required input fields and prevent users from accessing functions outside their assigned permissions. | Must |

### Non-Functional Requirements

| ID | Category | Measurable Requirement | Priority |
|---|---|---|---|
| NFR-01 | Performance | Using a demonstration dataset of up to 20 club listings and 100 membership requests, the system shall display club-directory search results within two seconds for at least 95% of 20 repeated test searches on the agreed test environment. | Must |
| NFR-02 | Usability and Accessibility | At least four out of five volunteer testers using fictional accounts shall complete the student application workflow without assistance. The main forms shall also be operable using a keyboard during a documented manual test. | Should |
| NFR-03 | Security and Privacy | All documented tests attempting to access another student's requests or manage requests for an unassigned club shall be denied. The prototype shall use only fictional or anonymised data. | Must |

## 4.7 Development Approach
The team will adopt an incremental development approach. The first increment will establish the project structure, user roles, and club directory. The second will implement membership requests and status tracking. The third will introduce club-leader decisions and administrator management. The final increment will focus on access control, testing, defect correction, and presentation preparation.

We chose incremental development because it allows us to build and test the system step by step. Since some requirements may change after receiving feedback, this approach makes it easier to improve the system without changing everything. It also helps us manage our time and identify problems early.

## 4.8 Team Plan and Risks

### Coordinator Roles

| Role | Assigned Member | Responsibilities |
|---|---|---|
| Process and Project Coordinator | Muneerah Almutairi | Coordinates the schedule, meetings, task tracking, repository organization, and submission checklist. |
| Requirements and Design Coordinator | Awrad Alshammeri  | Coordinates problem validation, requirements gathering, workflow modelling, and initial interface and data design. |
| Implementation and Quality Coordinator | Haya Almutairi | Coordinates implementation planning, integration, testing, defect tracking, and prototype quality checks. |

## 4.9 Sources, AI Use, and Contributions
### References
    Google. (n.d.). How to use Google Forms. Google Docs Editors Help. https://support.google.com/docs/answer/6281888

### Generative AI Use Disclosure
ChatGPT was used to help organize the proposal, draft requirements and workflows, identify possible comparison products, and improve clarity and structure.

The team reviewed and edited the AI-generated content to make sure it matched the project requirements and assignment instructions.

### Team Contributions

| Team Member | Contribution |
|---|---|
| Muneerah Almutairi | Team information (4.1), problem and users (4.2), team plan and risks (4.8). |
| Awrad Alshammeri | Existing solutions (4.3), scope and workflows (4.5), initial requirements (4.6). |
| Haya Almutairi | Proposed solution and justification (4.4), development approach (4.7), sources, AI use, and contributions (4.9). |
