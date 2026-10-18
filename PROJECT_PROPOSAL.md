
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
  University students often need to check multiple course syllabi to find important academic dates such as exams, quizzes, assignments, and projects. Since this information is spread across multiple documents, students spend extra time searching for important dates and may miss important deadlines or updates. Assessment dates may also change during the semester, making it difficult for students to stay informed and organize their study schedules. 
  
  Instructors may also face difficulties coordinating assessment dates with other courses, while the academic department may find it challenging to organize official examination schedules and reduce scheduling conflicts across the university.

  ### Why It Matters
  The ASACS system provides one personalized academic calendar that includes  important dates for all the student's courses. This makes it easier for students to stay organized, manage their academic schedules, keep track of important academic events, and reducing the chance of missing important deadlines. 

   ### Main Actors 
   1.student 
    
  the main user who selects courses, tracks deadlines, updates personal calendars.
  
   2.Instructor (faculty Member)
   
   the faculty member who uploads syllabi, reviews dates, sets quiz deadlines.
   
   3.Academic Department 
   
   the administrative team that oversees schedules and approves final exame

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


















