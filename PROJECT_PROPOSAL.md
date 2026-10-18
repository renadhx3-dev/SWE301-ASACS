
## 4.1 Team Information

**Project Title:** ASACS – Automatic Student Academic Calendar System

**Group Letter:** C

**Team Members:**
- Renad H Alotaibi
- Latefa Jazaa
- Nourah Almutairi

**GitHub Repository URL:** [SWE301-ASACS Repository](https://github.com/renadhx3-dev/SWE301-ASACS)

**Project Summary:**

ASACS is a web-based academic scheduling system that
automatically synchronizes assessment dates with students'
personal calendars and supports instructors and academic
departments in coordinating assessment schedules and
reducing scheduling conflicts.

## 4.2 Problem and users
### Problem:
   University students often need to check multiple course syllabi to find important academic dates such as exams, quizzes, assignment deadlines, and projects deadlines. Since this information is spread across different documents, students spend extra time searching for important dates and may miss deadlines or updates. Assessment dates may also change during the semester, making it difficult for students to stay informed and organize their study schedules. 
  
  Instructors may also face difficulties coordinating assessment dates with other courses, which can result in scheduling conflicts and increased academic workload for students. Similarly, academic department may find it challenging to organize official examination schedules while considering course difficulty, shared student enrollment, and the time between exams. 

  ### Why It Matters
  ASACS system provides students with a personalized academic calendar that includes important dates for all their selected courses. This helps students stay organized, manage their academic schedules, and reduce the risk of missing important deadlines.
  
 Additionally, ASACS supports instructors and academic departments by identifying scheduling conflicts and recommending suitable assessment dates based on student workload. This can help reduce academic pressure and improve examination planning.  
 
   ### Main Actors 
  **1. Student**

The primary user who selects courses and sections, tracks academic deadlines, receives notifications, and synchronizes academic events with personal calendar applications.

**2. Instructor (Faculty Member)**

The faculty member who uploads course syllabi, reviews suggested assessment dates, manages quizzes and assignment deadlines, and checks scheduling conflicts.

**3. Academic Department**

The administrative team responsible for reviewing examination scheduling recommendations, managing official examination periods, and approving final midterm and final examination schedules.


### 4.3 Existing Solutions

| Existing Process or Solution | Useful Features | Limitation for Users | Source |
| :--- | :--- | :--- | :--- |
| **Course Syllabi** | Outlines all course requirements, assignments, and exam expectations. | Students must manually check multiple documents, increasing the risk of missing updates or deadlines. | Course documents and syllabi |
| **Moodle Calendar** | Centralizes academic events inside the university's learning management system. | Primarily displays events manually created within Moodle (like online quizzes and assignments), so it may not automatically reflect overall syllabus timelines or synchronize directly with external personal calendars. | Official Moodle documentation |
| **Google Calendar** | Offers flexible personal scheduling and cross-device syncing. | Does not automatically pull academic assessments without manual entry or external integrations. | Official Google Calendar documentation |


## 4.4 Proposed Solution and Justification
  
#### Proposed Solution:
  ASACS is a web based system that extracts assessment information from course syllabi and suggest intial dates.
  It identifies scheduling conflicts and recommends suitable dates based on course difficulty, shared student enrollment, and available examination periods. 
  The system also allows students to integrate their academic schedules with their personal calendars, while instructors and academic departments manage and approve assessment dates according to their responsibilities.

#### Justification

  Unlike course syllabi and general calendar applications, ASACS combines assessment information with conflict detection and scheduling recommendations while supporting personal calendars. A small prototype is feasible for three students using simulated data and reusable software libraries.

## 4.5 Scope and Workflows

#### In Scope

  The initial ASACS prototype will include course and section selection, assessment date management, basic scheduling conflict detection, and recommendations for suitable assessment dates. Students will be able to view their academic schedules and export events to personal calendar applications.

#### Out of Scope

  The initial prototype will not include integration with live university databases, automatic verification of real student enrollments, or deployment as an official university-wide scheduling system. These capabilities may be considered in future development.

#### End-to-End Workflows

  Workflow 1: Student Academic Calendar
  A student selects their courses and sections. ASACS displays the relevant assessments and their dates, allowing the student to review the schedule and export academic events to a personal calendar.

  Workflow 2: Instructor Assessment Management
  An instructor provides assessment information for a course. ASACS identifies the relevant events and allows the instructor to review, confirm, or update their dates. The updated schedule becomes available to students enrolled in the relevant section.

  Workflow 3: Academic Exam Scheduling
  The academic department reviews assessment schedules and receives recommendations for reducing conflicts based on factors such as course difficulty and shared student enrollment. The department can review and approve the proposed exam dates, which are then reflected in students’ academic schedules.

## 4.6 Initial Requirements

#### Functional Requirements

##### FR1 – Course and Section Selection 
  The system shall allow students to select and update their courses and sections.

##### FR2 – Assessment Information Entry 
  The system shall allow instructors to provide assessment information for their courses.

##### FR3 – Assessment Identification 
  The system shall identify assessment dates from the provided course information.

##### FR4 – Assessment Date Management 
  The system shall allow instructors to review, confirm, and update assessment dates.

##### FR5 – Scheduling Conflict Detection 
  The system shall detect scheduling conflicts between assessments.

##### FR6 – Scheduling Recommendations 
  The system shall recommend suitable assessment dates based on scheduling constraints and academic workload factors.

##### FR7 – Examination Schedule Approval 
  The system shall allow academic departments to review and approve proposed examination dates.

##### FR8 – Calendar Export 
  The system shall allow students to export their academic schedules to personal calendar applications.

#### Non-Functional Requirements

##### NFR1 – Performance
  The system shall display a student’s academic schedule within 3 seconds under normal prototype testing conditions.

##### NFR2 – Usability
  At least 80% of test users shall be able to select their courses and view their academic schedules without assistance.

##### NFR3 – Reliability
  The system shall successfully save and retrieve assessment dates in at least 95% of repeated test operations.
  
## 4.7 Development Approach 

  our team chose **Incremental Development** to develop ASACS this approach allows us to divide the system into smaller, manageable increments. As each increment is developed, functional components can be tested and reviewed. we will the core calendar subscription functionality, followed by assessment schedule management and recommendations. after each increment, the team will conduct testing and collect feedback to issues and improve the system before proceeding the next increment. this approach is suitable for our team and the limited semester timeline since it will help us prioritize essential and manage development risks. We plan to reuse existing technologies, such as the iCalendar (ICS) standard and suitable software libraries, to reduce implementation complexity. Testing calendar subscriptions early will help us identify compatibility and synchronization issues before developing more advanced scheduling features. This approach also allows us to adjust later increments based on feedback while maintaining a realistic project scope.



## 4.8 Team Plan and Risks

### Team Roles and Responsibilities

| Team Member | Role and Responsibilities |
|---|---|
| Renad | **Team Coordination, System Design, and Quality Assurance:** Coordinates communication and collaboration among team members, contributes to system architecture and design, and oversees quality checks to ensure ASACS meets its requirements. |
| Latefa | **Implementation, Testing, and Workflows:** Implements system features, performs testing to verify system functionality, and documents the three end-to-end workflows of ASACS. |
| Nourah | **Requirements Engineering, Progress Tracking, and Milestones:** Defines and documents system requirements, monitors project progress, and tracks milestones and deadlines. |

All team members will collaborate on major project activities, review each other's work, and contribute throughout the development process.

### Project Milestones

| Milestone | Planned Activities | Expected Deliverable |
|---|---|---|
| 1. Project Proposal | Define the problem, users, project scope, initial requirements, and development approach. | Completed project proposal. |
| 2. Requirements and Models | Refine functional and non-functional requirements and document system workflows and models. | Requirements specification and system models. |
| 3. Design and Initial Prototype | Design the system architecture and develop an initial prototype focusing on course selection and personalized ICS calendar subscription. | System design and initial working prototype. |
| 4. Final Prototype, Testing, and Presentation | Integrate the core features, test calendar synchronization and scheduling functionality, document results, and prepare the final presentation. | Final prototype, testing results, and presentation. |

### Project Risks

| Risk | Potential Impact | Planned Response |
|---|---|---|
| Calendar Synchronization Issues | Delayed updates in external calendar applications may cause students to temporarily view outdated assessment dates. | Test ICS subscriptions and updates early, display the latest approved dates within ASACS, and inform users that calendar refresh timing depends on the provider. |
| Limited Development Time | Complex features may delay prototype completion or reduce the time available for testing. | Use incremental development, prioritize core features such as personalized calendar subscription, and monitor progress through project milestones. |
| Inaccurate Scheduling Recommendations | Incomplete course data or incorrect scheduling rules may produce unsuitable assessment date suggestions. | Test rule-based recommendations using simulated data and require academic department approval before publishing official exam dates. |






