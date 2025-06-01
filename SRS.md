![A blue and black logo AI-generated content may be
incorrect.](media/image1.png){width="5.30283573928259in"
height="2.138885608048994in"}

**CSE6224 SOFTWARE REQUIREMENTS ENGINEERING**

**TRIMESTER 2510**

**SOFTWARE REQUIREMENTS SPECIFICATIONS (SRS) --**

**CAMPUS WELLNESS PORTAL**

**LECTURE SECTION: TC2L**

**TUTORIAL SECTION: TT6L**

**GROUP: G2**

**GROUP MEMBERS:**

  ------------------------------------------------------------------------
     **ROLE**                    **NAME**                  **STUDENT ID**
  -------------- ----------------------------------------- ---------------
   Group Leader        Farah Hanim Binti Mohd Zamri          1221305625

   Group Member         Nur Thayiebah Binti Hamdan           1221305552

   Group Member     Mohammed Aamena Mohammed Abdulkarem      1221305728

   Group Member     Mohammed Yousef Mohammed Abdulkarem      1221305727
  ------------------------------------------------------------------------

Table of Contents

[Table of Tables [5](#table-of-tables)](#table-of-tables)

[1 Introduction [6](#introduction)](#introduction)

[1.1 Purpose [6](#purpose)](#purpose)

[1.2 Scope [6](#scope)](#scope)

[1.3 Product Overview [7](#product-overview)](#product-overview)

[1.3.1 Product Perspective (Relationship to Other Systems)
[8](#product-perspective-relationship-to-other-systems)](#product-perspective-relationship-to-other-systems)

[1.3.2 Product Functions (high-level)
[8](#product-functions-high-level)](#product-functions-high-level)

[1.3.3 User Characteristics
[9](#user-characteristics)](#user-characteristics)

[1.3.4 Limitations [10](#limitations)](#limitations)

[1.3.5 Definitions, Acronyms, and Abbreviations
[11](#definitions-acronyms-and-abbreviations)](#definitions-acronyms-and-abbreviations)

[2 References [14](#references)](#references)

[2.1 Document References
[14](#document-references)](#document-references)

[2.2 Standards and Regulations
[14](#standards-and-regulations)](#standards-and-regulations)

[3 Overall Description [14](#overall-description)](#overall-description)

[3.1 System Environment [15](#system-environment)](#system-environment)

[3.2 Operating Environment
[15](#operating-environment)](#operating-environment)

[3.3 Design and Implementation Constraints
[16](#design-and-implementation-constraints)](#design-and-implementation-constraints)

[4 Requirements [16](#requirements)](#requirements)

[4.1 Functional Requirements
[16](#functional-requirements)](#functional-requirements)

[4.1.1 Overview of System Functions
[16](#overview-of-system-functions)](#overview-of-system-functions)

[4.1.2 Use Case Diagram [18](#use-case-diagram)](#use-case-diagram)

[4.1.3 Use Case Descriptions
[19](#use-case-descriptions)](#use-case-descriptions)

[4.2 Interface Requirements
[70](#interface-requirements)](#interface-requirements)

[4.2.1 System Interfaces [70](#system-interfaces)](#system-interfaces)

[4.2.2 User Interfaces [70](#user-interfaces)](#user-interfaces)

[4.2.3 Hardware Interfaces
[71](#hardware-interfaces)](#hardware-interfaces)

[4.2.4 Software Interfaces
[71](#software-interfaces)](#software-interfaces)

[4.2.5 Communication Interfaces
[71](#communication-interfaces)](#communication-interfaces)

[4.3 Performance Requirements
[71](#performance-requirements)](#performance-requirements)

[4.4 Maintainability and Portability Requirements
[72](#maintainability-and-portability-requirements)](#maintainability-and-portability-requirements)

[4.5 Usability Requirements
[72](#usability-requirements)](#usability-requirements)

[4.6 Security Requirements
[73](#security-requirements)](#security-requirements)

[4.7 Logical Database Requirements
[74](#logical-database-requirements)](#logical-database-requirements)

[4.7.1 Entities [74](#entities)](#entities)

[4.7.2 Relationships [74](#relationships)](#relationships)

[4.7.3 Data Integrity Constraints
[75](#data-integrity-constraints)](#data-integrity-constraints)

[4.7.4 Security and Access Constraints
[75](#security-and-access-constraints)](#security-and-access-constraints)

[4.7.5 Performance and Optimization
[75](#performance-and-optimization)](#performance-and-optimization)

[5 Verification [76](#verification)](#verification)

[5.1 Verification Approach
[76](#verification-approach)](#verification-approach)

[5.2 Verification Criteria
[76](#verification-criteria)](#verification-criteria)

[5.3 Testing Strategy [77](#testing-strategy)](#testing-strategy)

[5.3.1 Test Levels and Scope
[77](#test-levels-and-scope)](#test-levels-and-scope)

[5.3.2 Test Artifacts and Deliverables
[78](#test-artifacts-and-deliverables)](#test-artifacts-and-deliverables)

[5.3.3 Test Environment [78](#test-environment)](#test-environment)

[5.3.4 Test Entry and Exit Criteria
[79](#test-entry-and-exit-criteria)](#test-entry-and-exit-criteria)

[6 Appendices [79](#appendices)](#appendices)

[6.1 Assumptions and Dependencies
[79](#assumptions-and-dependencies)](#assumptions-and-dependencies)

[6.1.1 Assumptions [79](#assumptions)](#assumptions)

[[6.1.2]{dir="rtl"} Dependencies [79](#dependencies)](#dependencies)

[6.2 Glossary [80](#glossary)](#glossary)

[6.3 Acronyms and Abbreviations
[81](#acronyms-and-abbreviations)](#acronyms-and-abbreviations)

[6.4 User Stories [81](#user-stories)](#user-stories)

[6.5 Class Diagram [83](#class-diagram)](#class-diagram)

[6.5.1 Purpose and Scope [83](#purpose-and-scope)](#purpose-and-scope)

[6.5.2 Classes and Responsibilities
[84](#classes-and-responsibilities)](#classes-and-responsibilities)

[6.5.3 Relationships [85](#relationships-1)](#relationships-1)

[6.5.4 Constraints and Business Rules
[86](#constraints-and-business-rules)](#constraints-and-business-rules)

[6.5.5 Traceability to Requirements
[86](#traceability-to-requirements)](#traceability-to-requirements)

[6.5.6 Compliance with ISO/IEC/IEEE 29148:2018
[87](#compliance-with-isoiecieee-291482018)](#compliance-with-isoiecieee-291482018)

[6.6 Requirement Traceability Matrix (RTM)
[87](#requirement-traceability-matrix-rtm)](#requirement-traceability-matrix-rtm)

[6.7 Supporting Materials
[88](#supporting-materials)](#supporting-materials)

[6.7.1 Kano Model Questionnaire Results
[88](#kano-model-questionnaire-results)](#kano-model-questionnaire-results)

[6.7.2 Kano Model Analysis
[97](#kano-model-analysis)](#kano-model-analysis)

[**6.7.3** Observation Checklist
[100](#observation-checklist)](#observation-checklist)

[6.7.4 Meeting Minutes and Brainstorm Notes
[102](#meeting-minutes-and-brainstorm-notes)](#meeting-minutes-and-brainstorm-notes)

Table of Figures

[Figure 1.1 -- Campus Wellness Portal Context Diagram
[8](#_Toc199101114)](#_Toc199101114)

[Figure 4.1 - Use Case Diagram [18](#_Toc199101115)](#_Toc199101115)

[Figure 4.2 - Login Sequence Diagram
[20](#_Toc199101116)](#_Toc199101116)

[Figure 4.3 - Login Activity Diagram
[21](#_Toc199101117)](#_Toc199101117)

[Figure 4.4 - View Available Medical Slots Sequence Diagram
[23](#_Toc199101118)](#_Toc199101118)

[Figure 4.5 - View Available Medical Slots Activity Diagram
[24](#_Toc199101119)](#_Toc199101119)

[Figure 4.6 - Book Medical Counselling Appointment Sequence Diagram
[26](#_Toc199101120)](#_Toc199101120)

[Figure 4.7 - Book Medical Counselling Appointment Activity Diagram
[27](#_Toc199101121)](#_Toc199101121)

[Figure 4.8 - Cancelling Appointment Sequence Diagram
[29](#_Toc199101122)](#_Toc199101122)

[Figure 4.9 - Cancelling Appointment Activity Diagram
[30](#_Toc199101123)](#_Toc199101123)

[Figure 4.10 - Reschedule Appointment Sequence Diagram
[32](#_Toc199101124)](#_Toc199101124)

[Figure 4.11 - Reschedule Appointment Activity Diagram
[33](#_Toc199101125)](#_Toc199101125)

[Figure 4.12 - View Counselling History Sequence Diagram
[35](#_Toc199101126)](#_Toc199101126)

[Figure 4.13 - View Counselling History Activity Diagram
[36](#_Toc199101127)](#_Toc199101127)

[Figure 4.14 - View Gym Available Sessions Sequence Diagram
[38](#_Toc199101128)](#_Toc199101128)

[Figure 4.15 - View Gym Available Sessions Activity Diagram
[39](#_Toc199101129)](#_Toc199101129)

[Figure 4.16 - Book Fitness Session Sequence Diagram
[41](#_Toc199101130)](#_Toc199101130)

[Figure 4.17 - Book Fitness Session Activity Diagram
[42](#_Toc199101131)](#_Toc199101131)

[Figure 4.18 - Track Wellness Progress Sequence Diagram
[44](#_Toc199101132)](#_Toc199101132)

[Figure 4.19 - Track Wellness Progress Activity Diagram
[45](#_Toc199101133)](#_Toc199101133)

[Figure 4.20 - Set Wellness Goals Sequence Diagram
[47](#_Toc199101134)](#_Toc199101134)

[Figure 4.21 - Set Wellness Goals Activity Diagram
[48](#_Toc199101135)](#_Toc199101135)

[Figure 4.22 - Get AI Wellness Tips Sequence Diagram
[50](#_Toc199101136)](#_Toc199101136)

[Figure 4.23 - Get AI Wellness Tips Activity Diagram
[51](#_Toc199101137)](#_Toc199101137)

[Figure 4.24 - Receive Notification Sequence Diagram
[54](#_Toc199101138)](#_Toc199101138)

[Figure 4.25 - Receive Notification Activity Diagram
[55](#_Toc199101139)](#_Toc199101139)

[Figure 4.26 - Manage Notification Sequence Diagram
[58](#_Toc199101140)](#_Toc199101140)

[Figure 4.27 - Manage Notification Activity Diagram
[59](#_Toc199101141)](#_Toc199101141)

[Figure 4.28 - View Student Wellness Report Sequence Diagram
[61](#_Toc199101142)](#_Toc199101142)

[Figure 4.29 - View Student Wellness Report Activity Diagram
[62](#_Toc199101143)](#_Toc199101143)

[Figure 4.30 - Manage Fitness Class Sequence Diagram
[64](#_Toc199101144)](#_Toc199101144)

[Figure 4.31 - Manage Fitness Class Activity Diagram
[65](#_Toc199101145)](#_Toc199101145)

[Figure 4.32 - Manage Medical Schedule Sequence Diagram
[67](#_Toc199101146)](#_Toc199101146)

[Figure 4.33 - Manage Medical Schedule Activity Diagram
[68](#_Toc199101147)](#_Toc199101147)

[Figure 6.1- UML Class Diagram For Campus Wellness Portal
[83](#_Toc199101148)](#_Toc199101148)

[Figure 6.2 - Questionnaire Board [88](#_Toc199101149)](#_Toc199101149)

[Figure 6.3 - Questionnaire Results (User Satisfaction With SSO)
[89](#_Toc199101150)](#_Toc199101150)

[Figure 6.4 - Questionnaire Results (User Satisfaction With Slots
Viewing) [89](#_Toc199101151)](#_Toc199101151)

[Figure 6.5 - Questionnaire Results (User Satisfaction With Appointment
Booking) [89](#_Toc199101152)](#_Toc199101152)

[Figure 6.6 - Questionnaire Results (User Satisfaction With
Cancel/Reschedule Appointment) [90](#_Toc199101153)](#_Toc199101153)

[Figure 6.7 - Questionnaire Results (User Satisfaction With History
Viewing) [90](#_Toc199101154)](#_Toc199101154)

[Figure 6.8 - Questionnaire Results (User Satisfaction With Tracking
Wellness Progress) [90](#_Toc199101155)](#_Toc199101155)

[Figure 6.9 - Questionnaire Results (User Satisfaction With Setting
Personal Goals) [91](#_Toc199101156)](#_Toc199101156)

[Figure 6.10 - Questionnaire Results (User Satisfaction With Provided
Tips) [91](#_Toc199101157)](#_Toc199101157)

[Figure 6.11 - Questionnaire Results (User Satisfaction With Sessions
Viewing) [91](#_Toc199101158)](#_Toc199101158)

[Figure 6.12 - Questionnaire Results (User Satisfaction With Sessions
Booking) [92](#_Toc199101159)](#_Toc199101159)

[Figure 6.13 - Questionnaire Results (User Satisfaction With
Notification And Reminders) [92](#_Toc199101160)](#_Toc199101160)

[Figure 6.14 - Questionnaire Results (User Satisfaction With
Gender-Specific Sessions Viewing) [92](#_Toc199101161)](#_Toc199101161)

[Figure 6.15 - Questionnaire Results (Dysfunction of SSO)
[93](#_Toc199101162)](#_Toc199101162)

[Figure 6.16 - Questionnaire Results (Dysfunction of Slots Viewing)
[93](#_Toc199101163)](#_Toc199101163)

[Figure 6.17 - Questionnaire Results (Dysfunction of Appointment
Booking) [93](#_Toc199101164)](#_Toc199101164)

[Figure 6.18 - Questionnaire Results (Dysfunction of Cancel/Rescheduling
Appointments) [94](#_Toc199101165)](#_Toc199101165)

[Figure 6.19 - Questionnaire Results (Dysfunction of History Viewing)
[94](#_Toc199101166)](#_Toc199101166)

[Figure 6.20 - Questionnaire Results (Dysfunction of Tracking Wellness
Progress) [94](#_Toc199101167)](#_Toc199101167)

[Figure 6.21 - Questionnaire Results (Dysfunction of Setting Personal
Goals) [95](#_Toc199101168)](#_Toc199101168)

[Figure 6.22 - Questionnaire Results (Dysfunction of Providing Tips)
[95](#_Toc199101169)](#_Toc199101169)

[Figure 6.23 - Questionnaire Results (Dysfunction of Sessions Viewing)
[95](#_Toc199101170)](#_Toc199101170)

[Figure 6.24 - Questionnaire Results (Dysfunction of Sessions Booking)
[96](#_Toc199101171)](#_Toc199101171)

[Figure 6.25 - Questionnaire Results (Dysfunction of Notification and
Reminders) [96](#_Toc199101172)](#_Toc199101172)

[Figure 6.26 - Questionnaire Results (Dysfunction of Gender-Specific
Sessions Viewing) [96](#_Toc199101173)](#_Toc199101173)

[Figure 6.27 - Kano Model Diagram [98](#_Toc199101174)](#_Toc199101174)

# Table of Tables

[Table 1.1 -- Definitions, Acronyms, and Abbreviations
[11](#_Toc199101175)](#_Toc199101175)

[Table 2.1 - Document References [14](#_Toc199101176)](#_Toc199101176)

[Table 2.2 - Standards and regulations
[14](#_Toc199101177)](#_Toc199101177)

[Table 4.1 - Login Use Case [19](#_Toc199101178)](#_Toc199101178)

[Table 4.2 - View Available Medical Slots Use Case
[22](#_Toc199101179)](#_Toc199101179)

[Table 4.3 - Book Medical Counselling Appointment Use Case
[25](#_Toc199101180)](#_Toc199101180)

[Table 4.4 - Cancel Appointment Use Case
[28](#_Toc199101181)](#_Toc199101181)

[Table 4.5 - Reschedule Appointment Use Case
[31](#_Toc199101182)](#_Toc199101182)

[Table 4.6 - View Counselling History Use Case
[34](#_Toc199101183)](#_Toc199101183)

[Table 4.7 - View Gym Available Sessions Use Case
[36](#_Toc199101184)](#_Toc199101184)

[Table 4.8 - Book Fitness Session Use Case
[40](#_Toc199101185)](#_Toc199101185)

[Table 4.9 - Track Wellness Progress Use Case
[43](#_Toc199101186)](#_Toc199101186)

[Table 4.10 - Set Wellness Goals Use Case
[46](#_Toc199101187)](#_Toc199101187)

[Table 4.11 - Get AI Wellness Tips Use Case
[48](#_Toc199101188)](#_Toc199101188)

[Table 4.12 - Receive Notification Use Case
[51](#_Toc199101189)](#_Toc199101189)

[Table 4.13 - Manage Notification Use Case
[56](#_Toc199101190)](#_Toc199101190)

[Table 4.14 - View Student Wellness Report Use Case
[60](#_Toc199101191)](#_Toc199101191)

[Table 4.15 - Manage Fitness Class Use Case
[62](#_Toc199101192)](#_Toc199101192)

[Table 4.16 - Manage Medical Schedule Use Case
[65](#_Toc199101193)](#_Toc199101193)

[Table 4.17 - Performance Requirements
[72](#_Toc199101194)](#_Toc199101194)

[Table 4.18 - Usability Requirements
[73](#_Toc199101195)](#_Toc199101195)

[Table 5.1 - Verification Criteria [76](#_Toc199101196)](#_Toc199101196)

[Table 5.2 - Test Entry And Exit Criteria
[79](#_Toc199101197)](#_Toc199101197)

[Table 6.1 - Glossary [80](#_Toc199101198)](#_Toc199101198)

[Table 6.2 - Acronyms and Abbreviations
[81](#_Toc199101199)](#_Toc199101199)

[Table 6.3 - Requirement Traceability Matrix
[87](#_Toc199101200)](#_Toc199101200)

[Table 6.4 - Kano Functional Classification with
Satisfaction-Functionality with Results
[97](#_Toc199101201)](#_Toc199101201)

[Table 6.5 - User Interaction and Behaviour Checklist
[100](#_Toc199101202)](#_Toc199101202)

[Table 6.6 - Scheduling and Appointment Management Checklist
[100](#_Toc199101203)](#_Toc199101203)

[Table 6.7 - Functional Workflow and CLiC Compliance Checklist
[100](#_Toc199101204)](#_Toc199101204)

[Table 6.8 - User Interface and Experience Checklist
[100](#_Toc199101205)](#_Toc199101205)

[Table 6.9 - Supplementary Video Observations Checklist
[101](#_Toc199101206)](#_Toc199101206)

[Table 6.10 - Summary of Bottlenecks and Recommendations
[101](#_Toc199101207)](#_Toc199101207)

# 

# Introduction 

## Purpose

> This Software Requirements Specification (SRS) defines the functional
> and non-functional requirements for the Campus Wellness Portal to be
> developed by Multimedia University (MMU). The primary purpose of this
> document is to provide a complete and consistent reference for all
> stakeholders ---including developers, testers, designers, and
> evaluators ---throughout the system development lifecycle.
>
> This system aims to address the fragmentation and inefficiency
> currently experienced by students when accessing wellness-related
> services such as medical bookings, counselling sessions, and fitness
> activities. By introducing a centralized and integrated digital
> platform, the Campus Wellness Portal will unify service scheduling,
> enhance user experience through personalized wellness insights, and
> ensure secure access via MMU's Single Sign-On (SSO).
>
> The specification of these requirements ensures that the resulting
> software aligns with MMU's strategic goal of promoting holistic
> student well-being and preventive care, while adhering to
> internationally recognized standards outlined in ISO/IEC/IEEE
> 29148:2018.

## Scope

> This document defines the scope of the Campus Wellness Portal (CWP), a
> software platform developed to centralize and streamline student
> access to health, counselling, and fitness services at Multimedia
> University (MMU).
>
> The CWP provides an integrated interface that connects with existing
> university infrastructure, including the CLiC Health and Counselling
> modules, the MMU Online Portal (Single Sign-On via OAuth 2.0), and the
> Campus Fitness Centre's scheduling systems. Designed for
> cross-platform use on desktop and mobile devices, the portal empowers
> users to manage wellness activities from a unified, responsive
> dashboard.
>
> The system's core functionality is driven by real student feedback and
> prioritization, ensuring alignment with authentic wellness needs and
> digital service expectations.
>
> The primary users of the CWP are MMU students. System administrators
> act as secondary users, overseeing appointment visibility and basic
> edits within the scheduling modules.
>
> In-scope features include:
>
> • Secure SSO authentication via the MMU Online Portal
>
> • Booking of medical appointments via CLiC Health
>
> • Counselling session scheduling and history access through CLiC
> Counselling
>
> • Real-time slot visibility for both health and counselling
> appointments
>
> • Booking and cancellation of fitness classes via the Campus Fitness
> Centre
>
> • Goal tracking modules for hydration, sleep, and physical activity
>
> • AI-generated wellness recommendations based on user data
>
> • Notifications and reminders via push and in-app alerts
>
> • Responsive web-based user interface, accessible across platforms
>
> Out-of-scope for this development phase:
>
> • Payment handling for services
>
> • Emergency or crisis medical features (e.g., ambulance requests)
>
> • Real-time chat with medical or counselling staff
>
> • Full administrative dashboards beyond appointments viewing/editing

## Product Overview

> The Campus Wellness Portal is a cross-platform software system that
> provides Multimedia University (MMU) students with centralized,
> seamless access to campus health, counselling, and fitness services.
> It enables users to book and manage medical appointments, counselling
> sessions, and fitness classes while tracking personalized wellness
> goals and receiving AI-generated health insights. The portal
> integrates with MMU's Single Sign-On (SSO) for secure access and
> interfaces with the CLiC Health and Counselling modules as well as the
> Campus Fitness Centre's scheduling system. Designed for accessibility
> across both desktop and mobile devices, the platform delivers a
> unified, real-time dashboard that simplifies and enhances student
> engagement with wellness resources.

### Product Perspective (Relationship to Other Systems)

> The Campus Wellness Portal operates as an integrated module within
> Multimedia University's broader digital ecosystem. It serves as a
> centralized platform through which students access health,
> counselling, and fitness services. The portal communicates with
> several external systems to support its core functionalities, as
> illustrates in Figure 1.
>
> Students interact directly with the portal to manage appointments, set
> wellness goals, and receive personalized tips. Authentication handles
> through the MMU Online Portal using a Single Sign-On (SSO) mechanism.
> The system interfaces with the Health Centre System to enable booking
> and viewing of medical appointments, and with the Fitness Centre
> System to allow scheduling and cancellation of fitness sessions.
> Administrative users can access the portal to view and update
> available time slots across services.
>
> This integration ensures seamless coordination between student actions
> and back-end service availability, consolidating previously fragmented
> wellness tools into a single, accessible platform.

<figure>
<img src="media/image2.png" style="width:6.26806in;height:3.05486in"
alt="A diagram of a campus wellness portal AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101114" class="anchor"></span>Figure 1.1
– Campus Wellness Portal Context Diagram</p></figcaption>
</figure>

### Product Functions (high-level)

> The Campus Wellness Portal supports student wellness through a range
> of integrated functions, organized into the following core domains:

- **Authentication and Access Control**

  - Authenticate students securely via MMU's Single Sign-On (SSO)
    mechanism (OAuth 2.0).

  - Maintain session integrity and role-based access.

- **Medical Appointment Management**

  - Book, view, reschedule, and cancel medical appointments.

  - Display real-time availability for medical slots.

- **Counselling Services Management**

  - Submit and manage counselling session requests.

  - View personal counselling history.

  - Ensure confidentiality of session records.

- **Fitness Class Scheduling**

  - Book, view, and cancel gym classes.

  - Show real-time schedules and availability.

  - Filter classes by gender when applicable.

- **Wellness Goal Tracking and Insights**

  - Set and monitor personal goals (e.g., hydration, sleep).

  - Visualize goal progress via dashboards.

  - Receive AI-generated personalized health tips.

- **Notifications and Reminders.**

  - Send automated reminders for upcoming sessions.

  - Allow user customization of notification preferences.

- **Unified Wellness Dashboard**

  - Aggregate key wellness data and alerts in a single view.

  - Provide downloadable reports for self-reflection.

- **Cross-Platform Accessibility**

  - Ensure consistent functionality and usability across web and mobile
    platforms.

  - Maintain a responsive, user-friendly interface.

- **Administrative Management Tools**

  - Enable staff to configure and manage service time slots.

  - Support operational scheduling across departments

### User Characteristics

> The primary users of the Campus Wellness Portal are undergraduate and
> postgraduate students at Multimedia University (MMU), spanning various
> faculties and academic disciplines. Users are generally comfortable
> with digital platforms and possess basic to intermediate levels of
> computer literacy. No specialized technical expertise is required to
> use the system.
>
> Most users primarily access services via smartphones, making mobile
> responsiveness and intuitive design essential. Users expect tasks such
> as appointment booking and class scheduling to be achievable within
> two to three clicks. This expectation emphasizes the need for a
> streamlined and user-friendly interface.
>
> Given the sensitivity of health and counselling data, users place a
> high priority on privacy and expect clear visibility into how their
> data is used. While features such as AI-generated tips and wellness
> recommendations are appreciated by some users, others prefer optional
> control over such functionalities.
>
> Overall, the system must accommodate a broad student population with
> varying schedules, preferences, and comfort levels with technology,
> requiring an accessible, responsive, and privacy-conscious design.

### Limitations

> The following limitations have been identified for the Campus Wellness
> Portal during the initial development phase:

- **Dependency on External Systems**: The system relies on real-time
  integration with the CLiC Health and Counselling modules and the
  Campus Fitness Centre scheduling system. Any downtime or data
  unavailability in these external systems will affect portal
  functionality.

- **No Offline Functionality**: The portal requires an active internet
  connection to operate. Offline access or synchronization is not
  supported in the current scope.

- **Exclusion of Emergency Features**: The portal is not designed for
  emergency response scenarios. It cannot be used to request urgent
  medical attention, ambulance dispatch, or crisis counselling
  intervention.

- **Limited Personalization of AI Tips**: AI-generated wellness
  recommendations are based on rule-based heuristics. Advanced
  personalization through machine learning is not implemented in the
  current release.

- **Mobile Optimization Limitations**: While the user interface is
  responsive, the initial release may provide a more complete experience
  on desktop browsers compared to mobile devices.

- **Partial Notification Preferences**: User control over notification
  preferences is limited to basic on/off toggles. Granular control
  (e.g., channel selection, frequency) may not be available in the MVP.

### Definitions, Acronyms, and Abbreviations 

> The following definitions clarify key terms and abbreviations used
> throughout this document:

  -----------------------------------------------------------------------
  **Term**               **Definition**
  ---------------------- ------------------------------------------------
  SRS                    Software Requirement Specification

  MMU                    Multimedia University

  SSO                    Single Sign-On -- A secure method of accessing
                         multiple systems with one login

  OAuth 2.0              An open standard for token-based authorization

  AI                     Artificial Intelligence -- Automated algorithms
                         that generate insights or recommendations

  UI                     User Interface -- The visual components a user
                         interacts with

  UX                     User Experience -- The overall experience and
                         usability of a system

  CWP                    Campus Wellness Portal

  UC                     Use Case -- A specific scenario of system
                         interaction

  HTTPS                  Hypertext Transfer Protocol Secure -- Secure
                         communication protocol

  TLS                    Transport Layer Security -- Cryptographic
                         protocol for data security

  REST API               Representational State Transfer API -- A web
                         standard for system communication

  HTML                   HyperText Markup Language -- Language used to
                         create web pages

  CSS                    Cascading Style Sheets -- Used for styling HTML
                         content

  JS                     JavaScript -- A scripting language for dynamic
                         content on the web

  LDAP                   Lightweight Directory Access Protocol -- Used
                         for directory services authentication

  SIS                    Student Information System -- Contains academic
                         and enrolment data

  DB                     Database -- Structured data storage used by
                         backend systems

  KPI                    Key Performance Indicator -- A metric to
                         evaluate system success or user goals

  RBAC                   Role-Based Access Control -- Authorization
                         mechanism based on user roles

  OTP                    One-Time Password -- A secure, time-limited code
                         used for login or verification

  OTA                    One-Time Authentication -- Used for sensitive or
                         privileged user actions

  PDPA                   Personal Data Protection Act -- Malaysian data
                         privacy legislation

  UAT                    User Acceptance Testing -- Final testing done by
                         actual users

  MVC                    Model-View-Controller -- A software architecture
                         pattern

  UUID                   Universally Unique Identifier -- A unique string
                         used as a database key

  WCAG                   Web Content Accessibility Guidelines --
                         Standards for making content accessible

  API                    Application Programming Interface -- Set of
                         rules for system-to-system communication

  DBMS                   Database Management System -- Software for
                         managing databases

  PII                    Personally Identifiable Information -- Data that
                         can identify an individual

  PHI                    Personal Health Information -- Sensitive
                         health-related data of individuals

  ReactJS                JavaScript library for building user interfaces

  PostgreSQL             Open-source relational database management
                         system

  HTML5                  Version 5 of the HyperText Markup Language

  CSS3                   Version 3 of Cascading Style Sheets

  CD                     Class Diagram -- A visual representation of
                         object relationships in software design

  ISO/IEC/IEEE           ISO/IEC/IEEE 29148:2018
  29148:2018             

  MedicalDB              Backend database containing medical appointments
                         and records

  FitnessDB              Backend database for gym class schedules and
                         bookings

  WellnessDB             Database storing personal goals and health
                         analytics

  PEP-8                  Python Enhancement Proposal 8 -- Official Python
                         code style guide

  MVP                    Minimum Viable Product -- Basic version of the
                         product with essential features

  SSL                    Secure Sockets Layer -- cryptographic protocol
                         for securing internet connections

  AES-256                Advanced Encryption Standard (256-bit key) --
                         strong data encryption algorithm

  GDPR                   General Data Protection Regulation -- European
                         law on personal data protection

  QA                     Quality Assurance -- practices ensuring software
                         meets requirements and standards

  JSON                   JavaScript Object Notation -- lightweight format
                         for data exchange

  SMS                    Short Message Service -- text messaging protocol
                         for mobile communication

  VPN                    Virtual Private Network -- encrypted connection
                         for secure remote access

  SMART                  Specific, Measurable, Achievable, Relevant,
                         Time-bound -- goal-setting framework

  HTTP                   Hypertext Transfer Protocol -- protocol used for
                         web data transmission

  UML                    Unified Modelling Language - diagramming
                         language used to model system structure and
                         behavior
  -----------------------------------------------------------------------

  : []{#_Toc199101175 .anchor}Table 1.1 -- Definitions, Acronyms, and
  Abbreviations

# References 

## Document References

  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Reference   **Title**                     **Author/Group**   **Source/Link**
  ID**                                                           
  ------------- ----------------------------- ------------------ -------------------------------------------------------------------------------------------------------------------------------
  DOC-1         TT6L_G2_ProjectPreliminary    Group TT6L_G2      [Project Preliminary](https://github.com/thayiebah/TT6L_G2_Requirements_Project/tree/main/ProjectPreliminary)

  DOC-2         TT6L_G2_ContextSources        Group TT6L_G2      [Context Objects](https://github.com/thayiebah/TT6L_G2_Requirements_Project/tree/main/ContextObjects)

  DOC-3         TT6L_G2_ElicitationPlan       Group TT6L_G2      [Elicitation
                                                                 Plan](https://github.com/thayiebah/TT6L_G2_Requirements_Project/blob/main/Elicitation/TT6L_G2_ElicitationPlan.docx)

  DOC-4         TT6L_G2_ElicitationExecuton   Group TT6L_G2      [Elicitation
                                                                 Execution](https://github.com/thayiebah/TT6L_G2_Requirements_Project/blob/main/Elicitation/TT6L_G2_ElicitationExecution.docx)

  DOC-5         Software Requirements         International      [ISO/IEC/IEEE 29148:2018](https://www.iso.org/standard/72089.html)
                Specification (SRS) --        Organization for   
                ISO/IEC/IEEE 29148:2018       Standardization    
  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

  : []{#_Toc199101176 .anchor}Table 2.1 - Document References

## Standards and Regulations

  --------------------------------------------------------------------------------------
  **Standard ID**   **Standard/Regulations**   **Publisher**     **Purpose/Relevance**
  ----------------- -------------------------- ----------------- -----------------------
  STD-1             ISO/IEC/IEEE 29148:2018 -- ISO/IEC/IEEE      Defines structure and
                    Systems and Software                         best practices for
                    Engineering -- Life Cycle                    software requirements
                    Processes -- Requirements                    specification (SRS).
                    Engineering                                  

  STD-2             OAuth 2.0 Authorization    IETF (RFC 6749)   Provides secure and
                    Framework                                    standardized protocol
                                                                 for Single Sign-On
                                                                 authentication.

  STD-3             General Data Protection    European Union    Ensures proper handling
                    Regulation (GDPR), EU                        of personal and
                    Regulation 2016/679                          sensitive student
                                                                 wellness data (if
                                                                 applicable).

  STD-4             **Malaysia Personal Data   Malaysian         Regulates the
                    Protection Act (PDPA)      Government / PDPD processing of personal
                    2010**                                       data in commercial
                                                                 transactions and
                                                                 protects users\'
                                                                 privacy.

  STD-5             **Web Content              World Wide Web    Ensures accessibility
                    Accessibility Guidelines   Consortium (W3C)  of the web portal for
                    (WCAG) 2.1 -- Level AA**                     all users, including
                                                                 those with
                                                                 disabilities.
  --------------------------------------------------------------------------------------

  : []{#_Toc199101177 .anchor}Table 2.2 - Standards and regulations

# Overall Description 

This section provides the high-level operational context, technical
environment, and architectural assumptions for the Campus Wellness
Portal. It offers an integrated view of the system's purpose, target
users, deployment environment, and external dependencies that inform
subsequent functional and non-functional requirements.

## System Environment

> Campus Wellness Portal is a web-based, holistic portal aimed at
> promoting the overall wellness of the students at Multimedia
> University (MMU). The portal is fully integrated with all the
> institutional services to offer an aggregated and seamless user
> experience. The portal is cross-device compatible, and the application
> has been developed to deliver the same performance and accessibility
> on desktops, tablets, and smartphones. Its strong architecture is
> centred on maintainability, scalability, and interoperability, and
> enables easy and secure user authentication using MMU\'s Single
> Sign-On (SSO) system. The system is modelled on the best software
> design and security principles and augments the university\'s vision
> for secure and stable digital services. The system follows established
> technology standards and security protocols, reflecting the
> university\'s dedication to providing dependable and protected online
> services for its academic community.

## Operating Environment 

> The Campus Wellness Portal will operate in a hybrid environment
> composed of institutional IT infrastructure and cloud services. It
> requires the following setup for deployment and operational support:
>
> **Client Environment:**

- Devices: Any modern web-enabled device (smartphones, tablets,
  desktops).

- Browsers: Latest versions of Chrome, Firefox, Safari, and Microsoft
  Edge.

- Connectivity: Stable internet access (minimum 10 Mbps recommended).

> **Server Environment:**

- **Backend:** Django framework (Python-based), adhering to REST API
  principles.

- **Frontend:** HTML5, CSS3, JavaScript with ReactJS framework for
  dynamic and responsive UI.

- **Database:** PostgreSQL for secure and scalable relational data
  storage.

- **APIs:** RESTful APIs for interaction between internal modules and
  external systems such as CLiC.

- **Hosting:** MMU\'s internal data centers or secured
  university-approved cloud provider.

<!-- -->

- **Network:** All network communication must be secured via HTTPS using
  TLS and operate on both the MMU intranet and general Internet with
  VPN/firewall protection and valid SSL certificates.

## Design and Implementation Constraints 

> The following constraints apply to the system\'s development and
> deployment:

- **Compliance:** The system must adhere to MMU's branding, data
  governance, accessibility, and cybersecurity policies.

- **Cross-platform Support:** Full responsiveness is required across
  devices, with consistent functionality on mobile and desktop
  environments.

- **Integration:** The portal must interact with existing legacy systems
  (e.g., CLiC, SIS) using API adapters or middleware.

- **Security:** Role-Based Access Control (RBAC) is mandatory for access
  to sensitive data (e.g., counselling or medical information).

- **Performance Expectations:** Real-time features such as appointment
  slot availability must update dynamically without degrading response
  time.

# Requirements 

This section describes the detailed system requirements needed to
develop the Campus Wellness Portal. These requirements follow the
ISO/IEC/IEEE 29148:2018 standards and meet stakeholders needs. The list
includes functional, interface, and non-functional needs. Each
requirement ensures clarity, traceability, completeness, and the ability
to test it during the entire system lifecycle.

## Functional Requirements 

### Overview of System Functions

> The Campus Wellness Portal is designed to serve as a centralized
> digital platform through which MMU students can access, monitor, and
> manage services related to their physical and mental well-being. It
> interfaces with existing institutional systems such as health
> services, counselling center, and fitness management tools. The
> system's functional scope includes:
>
> **Authentication & Access Control**: 
>
> Secure user access is ensured by MMU Single Sign-On (SSO) by
> authentication and access control. Data accessibility and feature
> visibility are controlled by Role-Based Access Control (RBAC), which
> is based on roles such Administrator and Student.
>
> **Medical Appointment Management**:
>
> Students can view real-time availability of medical consultation
> slots. They are able to book, cancel, and reschedule medical or
> counselling appointments. The system sends confirmation notifications
> for all appointment-related activities.
>
> **Counselling Services Management**: 
>
> Users can access their personal counselling history and manage future
> health-related appointments through the portal.
>
> **Fitness Class Integration**: 
>
> The system provides real-time visibility of available fitness
> sessions, including options to filter by gender. Students can book
> fitness classes via the platform.
>
> **Wellness Goal Management**:
>
> Students are enabled to define, set, and track personal wellness
> goals. Progress toward these goals is visualized through interactive
> dashboards.
>
> **AI-Based Personalized Recommendations**:
>
> The system offers customized wellness tips and motivational prompts,
> generated based on user interaction data and progress towards set
> goals.
>
> **Notification & Alerts System**:
>
> The system sends notifications via email and SMS. These notifications
> include reminders for upcoming bookings, confirmations, rescheduling
> alerts, updates on goal progress, and other relevant activities.
>
> **Administrative Operations**:
>
> Administrators can manage user notifications, schedules, and system
> logs. Additionally, the system supports the generation of wellness
> reports for administrative review.
>
> Each of these functions is supported by secure communication protocols
> (HTTPS/TLS), real-time data synchronization, mobile-friendly interface
> designs, and continuous backend monitoring to ensure reliability,
> availability, and usability.

### Use Case Diagram

<figure>
<img src="media/image3.png" style="width:6.01667in;height:5.61667in"
alt="A diagram of a health care system AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101115" class="anchor"></span>Figure 4.1
- Use Case Diagram</p></figcaption>
</figure>

**Figure 4.1** illustrates the use case diagram for the Campus Wellness
Portal, depicting interactions between system actors and core
functionalities. The primary actors are the **Student** and
the **Admin**. The Student interacts with the system to book and manage
medical counselling and fitness sessions, track wellness progress, and
access personalized recommendations. The Admin performs system oversight
tasks, including the management of medical schedules, student wellness
reports, notifications, and fitness classes.

The diagram also includes external systems, namely the **Health Center
System** and the **Fitness Center System**, which support medical
appointment handling and fitness class scheduling, respectively. Use
cases such as *Book Medical Counselling Appointment* incorporate related
actions like *Cancel Appointment* and *Reschedule Appointment* through
\"include\" relationships. Similarly, *Track Wellness
Progress* includes *Set Wellness Goals* and *Get AI Wellness Tips*.

This diagram provides a visual representation of system functionality
and actor interactions, supporting the identification of functional
requirements.

### Use Case Descriptions

#### Login

+-----------------------------+------------------+---------------------------------------------------------------------------+
| **No.**                     | **Section**      | **Context/Explanation**                                                   |
+:===============+:===========+:=================+:==========================================================================+
| **ID**         | 1.1        | Use Case ID      | UC01                                                                      |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 1.2        | Name             | Login                                                                     |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Management** | 2.1        | Author(s)        | Farah Hanim binti Mohd Zamri                                              |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 2.2        | Version          | 1.0                                                                       |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Context**    | 3.1        | Source(s)        | Questionnaire (Microsoft Forms)                                           |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Use Case     | 4.1        | Short            |   ----------------------------------------------------------------------- |
| Definition**   |            | Description      |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |   The user enters their credentials and logs into the portal via Single   |
|                |            |                  |   Sign-On (OAuth 2.0).                                                    |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.2        | Associated       | - G5.2 -- MMU Single Sign-On (SSO)                                        |
|                |            | Goal(s)          |                                                                           |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.3        | Primary Actor(s) | Student                                                                   |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.4        | Other Actor(s)   | MMU Online Portal                                                         |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.5        | Precondition(s)  | - The student must have a valid university account.                       |
|                |            |                  |                                                                           |
|                |            |                  | - The SSO Service must be available and responsive.                       |
|                |            |                  |                                                                           |
|                |            |                  | - Internet connection is available.                                       |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.5        | Postcondition(s) | - On success: Student is redirected to their personalized dashboard.      |
|                |            |                  |                                                                           |
|                |            |                  | - On failure: An error message is displayed                               |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.6        | Result           | User is authenticated and granted access to the Campus Wellness Portal.   |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.7        | Main Scenario    | 1.  Student navigates to the login page.                                  |
|                |            |                  |                                                                           |
|                |            |                  | 2.  Student enters username and password.                                 |
|                |            |                  |                                                                           |
|                |            |                  | 3.  System validates input format.                                        |
|                |            |                  |                                                                           |
|                |            |                  | 4.  Credentials sent to MMU Online Portal via OAuth 2.0.                  |
|                |            |                  |                                                                           |
|                |            |                  | 5.  If authentication succeeds, the system redirects to the dashboard.    |
|                |            |                  |                                                                           |
|                |            |                  | 6.  If authentication succeeds, the system redirects to the dashboard.    |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.8        | Alternate        | - Input fields are empty: System prompts user to fill in all fields.      |
|                |            | Scenario(s)      |                                                                           |
|                |            |                  | - Slow response from MMU SSO: System displays "Authenticating..."         |
|                |            |                  |   message.                                                                |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.9        | Exception        | - Invalid Credentials Entered                                             |
|                |            | Scenario(s)      |                                                                           |
|                |            |                  | - SSO Service Unavailable                                                 |
+----------------+------------+------------------+---------------------------------------------------------------------------+

: []{#_Toc199101178 .anchor}Table 4.1 - Login Use Case

#####  Sequence Diagram

![[]{#_Toc199101116 .anchor}Figure 4.2 - Login Sequence
Diagram](media/image4.png){width="6.268055555555556in"
height="3.94375in"}

**Figure 4.2** is the sequence diagram for Login portraying the dialogue
among various entities taking part in the logging process, i.e., the
Student, Login Page, SSO Module, MMU Online Portal, and Dashboard. The
process begins with the inputting of the student\'s credentials on the
login page, which are verified. The alt block is used to verify if the
input is complete or not. When the input is complete, then the
credentials are forwarded to the SSO module, which further passes them
to the MMU Online Portal for verification. Once a response token is
received, access is provided, and the user is redirected to the
dashboard or an error page if something goes wrong. If there\'s partial
input, the system will bypass the authentication call and immediately
return with a request for completion of missing fields. This diagram is
perfect in specifying data flow and decision-making during the login,
and all the various scenarios are covered.

##### Activity Diagram

![[]{#_Toc199101117 .anchor}Figure 4.3 - Login Activity
Diagram](media/image5.png){width="6.213098206474191in"
height="4.401388888888889in"}

**Figure 4.3** portrays the Login activity diagram that illustrates the
steps to be taken in order to log into the Campus Wellness Portal as a
student. This follows after the input of the login
credentials---username and password---and clicking the login button. The
system first verifies if the credentials are both available. The system
immediately provides an error message requesting the user to enter both
fields in the event that either is left blank. The system proceeds to
forward the credentials to the MMU Online Portal for authentication
through OAuth 2.0 in the event that the credentials are correct.
Feedback that authentication is in progress is provided to the user
during this process. After authentication, the student is redirected to
the student dashboard. If authentication fails because of incorrect
submission of credentials, an error message is shown to try again. This
sequence diagram follows successful and failed login attempts and
incompleteness feedback.

#### View Available Medical Slots

+----------------------------+------------------+------------------------------+
| **No.**                    | **Section**      | **Context/Explanation**      |
+:===============+:==========+:=================+:=============================+
| **ID**         | 1.1       | Use Case ID      | UC02                         |
|                +-----------+------------------+------------------------------+
|                | 1.2       | Name             | View Available Medical Slots |
+----------------+-----------+------------------+------------------------------+
| **Management** | 2.1       | Author(s)        | Mohammed Yousef Mohammed     |
|                |           |                  | Abdulkarem                   |
|                +-----------+------------------+------------------------------+
|                | 2.2       | Version          | 1.0                          |
+----------------+-----------+------------------+------------------------------+
| **Context**    | 3.1       | Source(s)        | Questionnaire (Microsoft     |
|                |           |                  | Forms), Observation          |
+----------------+-----------+------------------+------------------------------+
| **Use Case     | 4.1       | Short            | Enables students to view     |
| Definition**   |           | Description      | real-time availability of    |
|                |           |                  | medical consultation slots   |
|                |           |                  | via the Campus Wellness      |
|                |           |                  | Portal.                      |
|                +-----------+------------------+------------------------------+
|                | 4.2       | Associated       | - G1.1 -- CLiC Integration   |
|                |           | Goal(s)          |                              |
|                +-----------+------------------+------------------------------+
|                | 4.3       | Primary Actor(s) | Student                      |
|                +-----------+------------------+------------------------------+
|                | 4.4       | Other Actor(s)   | Admins                       |
|                +-----------+------------------+------------------------------+
|                | 4.5       | Precondition(s)  | \- Student is logged in and  |
|                |           |                  | authenticated via the Campus |
|                |           |                  | Wellness Portal.\            |
|                |           |                  | - Backend appointment        |
|                |           |                  | service is accessible and    |
|                |           |                  | operational.                 |
|                +-----------+------------------+------------------------------+
|                | 4.6       | Postcondition(s) | \- Student views an          |
|                |           |                  | up-to-date list of available |
|                |           |                  | slots, filtered as per       |
|                |           |                  | chosen criteria.             |
|                +-----------+------------------+------------------------------+
|                | 4.7       | Result           | The system displays a list   |
|                |           |                  | of available medical slots   |
|                |           |                  | with date, time, and doctor  |
|                |           |                  | details to be viewed by the  |
|                |           |                  | user.                        |
|                +-----------+------------------+------------------------------+
|                | 4.8       | Main Scenario    | 1\. Student accesses the     |
|                |           |                  | "View Medical Slots"         |
|                |           |                  | interface.\                  |
|                |           |                  | 2. System validates the user |
|                |           |                  | session via the              |
|                |           |                  | Authentication Service.\     |
|                |           |                  | 3. System queries the        |
|                |           |                  | Appointment Service to       |
|                |           |                  | retrieve available slots     |
|                |           |                  | (date, time, doctor,         |
|                |           |                  | consultation type).\         |
|                |           |                  | 4. System presents slots in  |
|                |           |                  | a structured, user-friendly  |
|                |           |                  | format.\                     |
|                |           |                  | 5. Student optionally        |
|                |           |                  | applies filters (e.g., date, |
|                |           |                  | provider, type).\            |
|                |           |                  | 6. System updates the        |
|                |           |                  | displayed list based on      |
|                |           |                  | selected filters.\           |
|                |           |                  | 7. Student may proceed to    |
|                |           |                  | initiate a booking (triggers |
|                |           |                  | UC03).                       |
|                +-----------+------------------+------------------------------+
|                | 4.9       | Alternative      | \- 5a. No Filters Applied:\  |
|                |           | Scenario(s)      |  5a1. System defaults to     |
|                |           |                  | showing all slots available  |
|                |           |                  | in the next 7 days.\         |
|                |           |                  | - 6a. No Slots Available:\   |
|                |           |                  |  6a1. System displays a      |
|                |           |                  | message: "No available       |
|                |           |                  | appointments at this time."\ |
|                |           |                  | - 7a. Backend Unavailable or |
|                |           |                  | Timeout:\                    |
|                |           |                  |  7a1. System displays an     |
|                |           |                  | error message indicating     |
|                |           |                  | connectivity or service      |
|                |           |                  | maintenance issues.          |
+----------------+-----------+------------------+------------------------------+

: []{#_Toc199101179 .anchor}Table 4.2 - View Available Medical Slots Use
Case

##### Sequence Diagram

<figure>
<img src="media/image6.png" style="width:6.26806in;height:3.31111in"
alt="A diagram of a diagram AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101118" class="anchor"></span>Figure 4.4
- View Available Medical Slots Sequence Diagram</p></figcaption>
</figure>

**Figure 4.4** presents the sequence diagram that describes the
operational flow for the \"View Medical Slots\" use case within the
Campus Wellness Portal. The sequence begins when the Student accesses
the relevant page, prompting the Campus Wellness Portal to verify the
login status via the Authentication Service. Upon successful
authentication, the portal sends a request to the Medical Center Service
for available medical slots, which then queries the MedicalDB and
returns the data. If available slots are found, they are displayed to
the Student; otherwise, an appropriate notification message is shown.
The diagram also depicts an optional interaction where the Student
applies filters to narrow down the slot list. In such cases, the portal
forwards the filter parameters to the Medical Center Service, which
performs a filtered query against the MedicalDB and returns the refined
results for presentation. This sequence diagram effectively illustrates
the step-by-step communication and system responsibilities required to
support the viewing of medical slot availability.

##### Activity Diagram

<figure>
<img src="media/image7.png" style="width:6.26806in;height:4.37639in"
alt="A screenshot of a computer AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101119" class="anchor"></span>Figure 4.5
- View Available Medical Slots Activity Diagram</p></figcaption>
</figure>

**Figure 4.5** presents an activity diagram that outlines the workflow
for a Student to \"View Medical Slots\" within the Campus Wellness
Portal, detailing interactions with the Medical Centre Service and the
Medical Database. The process begins when the Student opens the relevant
page, prompting the Campus Wellness Portal to verify the login status;
if the user is not authenticated, the system redirects to the login
page. Upon successful authentication, the portal initiates a request to
the Medical Service Centre to retrieve available appointment slots,
which queries the Medical Database and returns the slot data. The Campus
Wellness Portal then displays the available slots to the Student. The
Student may optionally apply filters such as time or doctor, in which
case the system processes the criteria and updates the results
accordingly. If no matching slots are found based on the selected
filters, the system displays an appropriate error message. This diagram
captures the key decision points, data flow, and system responsibilities
involved in supporting medical slot visibility for students.

#### Book Medical Counselling Appointment

+----------------------------+------------------+------------------------------+
| **No.**                    | **Section**      | **Context/Explanation**      |
+:===============+:==========+:=================+:=============================+
| **ID**         | 1.1       | Use Case ID      | UC03                         |
|                +-----------+------------------+------------------------------+
|                | 1.2       | Name             | Book Medical Counselling     |
|                |           |                  | Appointment                  |
+----------------+-----------+------------------+------------------------------+
| **Management** | 2.1       | Author(s)        | Mohammed Yousef Mohammed     |
|                |           |                  | Abdulkarem                   |
|                +-----------+------------------+------------------------------+
|                | 2.2       | Version          | 1.0                          |
+----------------+-----------+------------------+------------------------------+
| **Context**    | 3.1       | Source(s)        | Questionnaire (Microsoft     |
|                |           |                  | Forms), Observation          |
+----------------+-----------+------------------+------------------------------+
| **Use Case     | 4.1       | Short            | Allows students to reserve a |
| Definition**   |           | Description      | medical or counselling       |
|                |           |                  | consultation slot through    |
|                |           |                  | the portal.                  |
|                +-----------+------------------+------------------------------+
|                | 4.2       | Associated       | - G1.1 -- CLiC Integration   |
|                |           | Goal(s)          |                              |
|                |           |                  | - G1.2 -- Manage             |
|                |           |                  |   Appointments               |
|                |           |                  |                              |
|                |           |                  | - G2.1 -- Request            |
|                |           |                  |   Counselling Session        |
|                +-----------+------------------+------------------------------+
|                | 4.3       | Primary Actor(s) | Student                      |
|                +-----------+------------------+------------------------------+
|                | 4.4       | Other Actor(s)   | Admins                       |
|                +-----------+------------------+------------------------------+
|                | 4.5       | Precondition(s)  | \- Student is authenticated  |
|                |           |                  | via the portal.\             |
|                |           |                  | - Selected slot is confirmed |
|                |           |                  | available in real-time.      |
|                +-----------+------------------+------------------------------+
|                | 4.6       | Postcondition(s) | \- Appointment is            |
|                |           |                  | successfully booked and      |
|                |           |                  | confirmed.\                  |
|                |           |                  | - Student receives           |
|                |           |                  | confirmation via email and   |
|                |           |                  | system notification.         |
|                +-----------+------------------+------------------------------+
|                | 4.7       | Result           | The system confirms and      |
|                |           |                  | records the user's medical   |
|                |           |                  | counselling appointment in   |
|                |           |                  | the schedule.                |
|                +-----------+------------------+------------------------------+
|                | 4.8       | Main Scenario    | 1\. Student navigates to     |
|                |           |                  | "Book Medical Appointment"   |
|                |           |                  | interface.\                  |
|                |           |                  | 2. System verifies the       |
|                |           |                  | session via Authentication   |
|                |           |                  | Service.\                    |
|                |           |                  | 3. System displays updated   |
|                |           |                  | available consultation       |
|                |           |                  | slots.\                      |
|                |           |                  | 4. Student selects a         |
|                |           |                  | preferred slot.\             |
|                |           |                  | 5. System checks for         |
|                |           |                  | conflicts and confirms       |
|                |           |                  | availability.\               |
|                |           |                  | 6. System reserves the slot  |
|                |           |                  | and updates the backend      |
|                |           |                  | Appointment Service.\        |
|                |           |                  | 7. Notification Service      |
|                |           |                  | sends a booking confirmation |
|                |           |                  | email.\                      |
|                |           |                  | 8. Student sees a success    |
|                |           |                  | message on the screen.       |
|                +-----------+------------------+------------------------------+
|                | 4.9       | Alternative      | \- 4a. Slot No Longer        |
|                |           | Scenario(s)      | Available:\                  |
|                |           |                  |  4a1. System notifies:       |
|                |           |                  | "Selected slot is no longer  |
|                |           |                  | available---please choose    |
|                |           |                  | another."\                   |
|                |           |                  | - 5a. Time Conflict with     |
|                |           |                  | Existing Appointment:\       |
|                |           |                  |  5a1. System prompts student |
|                |           |                  | to resolve scheduling        |
|                |           |                  | conflict.\                   |
|                |           |                  | - 6a. Booking Failure        |
|                |           |                  | (System Error):\             |
|                |           |                  |  6a1. System alerts student  |
|                |           |                  | and advises retry.           |
+----------------+-----------+------------------+------------------------------+

: []{#_Toc199101180 .anchor}Table 4.3 - Book Medical Counselling
Appointment Use Case

##### Sequence Diagram

<figure>
<img src="media/image8.png" style="width:6.26806in;height:2.90139in"
alt="A diagram of a company AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101120" class="anchor"></span>Figure 4.6
- Book Medical Counselling Appointment Sequence Diagram</p></figcaption>
</figure>

**Figure 4.6** illustrates a detailed sequence diagram describing the
process for a Student to book a medical appointment via the Campus
Wellness Portal. The interaction begins when the Student initiates a
booking request, prompting the portal to authenticate the user\'s
credentials through the Authentication Service. Upon successful
authentication, the portal retrieves and displays available medical
slots by querying the Medical DB via the Medical Centre Service. Once
the Student selects a preferred slot, the portal sends an appointment
booking request to the Medical Center Service, which verifies the
slot\'s availability. Two alternative flows are depicted: if the slot is
available, it is reserved in the Medical DB, the booking is confirmed to
the Student through the portal, and the Notification Service is
triggered to send a confirmation email; if the slot is unavailable, the
Student is notified accordingly and offered the option to join a
waitlist. This sequence diagram effectively captures the complete flow,
decision points, and system responsibilities involved in the medical
appointment booking process.

##### Activity Diagram

<figure>
<img src="media/image9.png" style="width:6.26806in;height:5.23056in"
alt="A diagram of a flowchart AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101121" class="anchor"></span>Figure 4.7
- Book Medical Counselling Appointment Activity Diagram</p></figcaption>
</figure>

**Figure 4.7** presents an activity diagram that meticulously outlines
the workflow for a Student to book an appointment via the Campus
Wellness Portal, involving the Medical Center Service and the
Appointment Database. The process begins with the Student opening the
\"Book Appointment\" page, after which the Campus Wellness Portal
verifies the user\'s login status, redirecting to a login page if the
user is not authenticated. If logged in, the portal proceeds to retrieve
available slots by prompting the Medical Center Service to query the
Appointment Database, which then returns the available slot data back to
the portal for display to the student. Following the display, the
Student selects a preferred slot and confirms the booking, which
triggers the Campus Wellness Portal to send a booking request to the
Medical Center Service. The Medical Center Service then attempts to
reserve the selected slot in the Appointment Database. The Medical
Centre Service then makes a critical decision: if the reservation is
successful, it sends a success confirmation back to the portal; if not,
it sends an error. Before the procedure is finished, the Campus Wellness
Portal assesses the booking outcome and displays an error message for
unsuccessful efforts or a confirmation message for successful bookings.

#### Cancel Appointment

+--------------------------+------------------+----------------------------------+
| **No.**                  | **Section**      | **Context/Explanation**          |
+:===============+:========+:=================+:=================================+
| **ID**         | 1.1     | Use Case ID      | UC04                             |
|                +---------+------------------+----------------------------------+
|                | 1.2     | Name             | Cancel Appointment               |
+----------------+---------+------------------+----------------------------------+
| **Management** | 2.1     | Author(s)        | Mohammed Yousef Mohammed         |
|                |         |                  | Abdulkarem                       |
|                +---------+------------------+----------------------------------+
|                | 2.2     | Version          | 1.0                              |
+----------------+---------+------------------+----------------------------------+
| **Context**    | 3.1     | Source(s)        | Questionnaire (Microsoft Forms)  |
+----------------+---------+------------------+----------------------------------+
| **Use Case     | 4.1     | Short            | Enables students to cancel a     |
| Definition**   |         | Description      | confirmed appointment and        |
|                |         |                  | release the slot for others.     |
|                +---------+------------------+----------------------------------+
|                | 4.2     | Associated       | - G1.1 -- CLiC Integration       |
|                |         | Goal(s)          |                                  |
|                |         |                  | - G1.2 -- Manage Appointments    |
|                +---------+------------------+----------------------------------+
|                | 4.3     | Primary Actor(s) | Student                          |
|                +---------+------------------+----------------------------------+
|                | 4.4     | Other Actor(s)   | Admin                            |
|                +---------+------------------+----------------------------------+
|                | 4.5     | Precondition(s)  | \- Student is authenticated via  |
|                |         |                  | the portal.\                     |
|                |         |                  | - At least one upcoming          |
|                |         |                  | appointment is present in the    |
|                |         |                  | student's schedule.              |
|                +---------+------------------+----------------------------------+
|                | 4.6     | Postcondition(s) | \- Appointment is successfully   |
|                |         |                  | cancelled.\                      |
|                |         |                  | - Slot becomes available for     |
|                |         |                  | others.\                         |
|                |         |                  | - Student receives a             |
|                |         |                  | cancellation confirmation        |
|                |         |                  | notification.                    |
|                +---------+------------------+----------------------------------+
|                | 4.7     | Result           | The system removes the selected  |
|                |         |                  | appointment from the user's      |
|                |         |                  | schedule and updates the         |
|                |         |                  | availability of that slot.       |
|                +---------+------------------+----------------------------------+
|                | 4.8     | Main Scenario    | 1\. Student accesses "My         |
|                |         |                  | Appointments" dashboard.\        |
|                |         |                  | 2. System validates the          |
|                |         |                  | student's session.\              |
|                |         |                  | 3. Student selects "Cancel"      |
|                |         |                  | button on appointment to         |
|                |         |                  | cancel.\                         |
|                |         |                  | 4. System prompts for            |
|                |         |                  | cancellation confirmation.\      |
|                |         |                  | 5. Student confirms.\            |
|                |         |                  | 6. System cancels the            |
|                |         |                  | appointment and updates          |
|                |         |                  | scheduling records.\             |
|                |         |                  | 7. Notification Service sends    |
|                |         |                  | cancellation confirmation        |
|                |         |                  | email.\                          |
|                |         |                  | 8. System displays confirmation  |
|                |         |                  | message.                         |
|                +---------+------------------+----------------------------------+
|                | 4.9     | Alternative      | \- 3a. No Appointments to        |
|                |         | Scenario(s)      | Cancel:\                         |
|                |         |                  |  3a1. System displays: "You have |
|                |         |                  | no upcoming appointments."\      |
|                |         |                  | - 5a. Cancellation Within Short  |
|                |         |                  | Notice Window (\<2 hours):\      |
|                |         |                  |  5a1. System warns of            |
|                |         |                  | short-notice cancellation.\      |
|                |         |                  |  5a2. Student may proceed or     |
|                |         |                  | abort cancellation.              |
+----------------+---------+------------------+----------------------------------+

: []{#_Toc199101181 .anchor}Table 4.4 - Cancel Appointment Use Case

##### Sequence Diagram

<figure>
<img src="media/image10.png" style="width:6.26806in;height:2.84861in"
alt="A diagram of a project AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101122" class="anchor"></span>Figure 4.8
- Cancelling Appointment Sequence Diagram</p></figcaption>
</figure>

**Figure 4.8** presents a sequence diagram illustrating the process for
a Student to cancel an appointment via the Campus Wellness Portal. The
sequence begins when the Student navigates to the \"My Appointments\"
page, prompting the Campus Wellness Portal to validate the session
through the Authentication Service. Once authenticated, the Student
selects an appointment and initiates a cancellation request, which the
portal forwards---along with the appointment ID---to the Medical Center
Service. The Medical Center Service then performs a cancellation
operation in the MedicalDB. Two flows are depicted: if the appointment
is found and is eligible for cancellation, the MedicalDB confirms the
cancellation, the Medical Center Service triggers the Notification
Service to send a cancellation email, and a success message is returned
to the portal for display. If the appointment is not found or cannot be
cancelled (e.g., it is in the past), the Medical Center Service returns
an error, and the portal displays an appropriate message to the Student.
This diagram captures the full operational flow, conditional logic, and
system responsibilities involved in cancelling an appointment.

##### Activity Diagram

<figure>
<img src="media/image11.png" style="width:6.26806in;height:3.96528in"
alt="A screenshot of a computer AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101123" class="anchor"></span>Figure 4.9
- Cancelling Appointment Activity Diagram</p></figcaption>
</figure>

**Figure 4.9** presents an activity diagram that outlines the workflow
for a Student to cancel an appointment within the Campus Wellness
Portal, involving interactions with the Medical Center Service and the
Appointment Database. The process begins when the Student navigates to
the \"My Appointments\" page. The system first checks whether the
Student is authenticated; if not, it redirects the user to the login
page for authentication. Upon successful login, the portal retrieves the
Student's list of upcoming appointments. The Student then selects an
appointment to cancel, prompting the Campus Wellness Portal to send a
cancellation request to the Medical Center Service. This service
attempts to delete the specified appointment from the Appointment
Database. A decision point follows: if the deletion is successful, the
system confirms the cancellation and sends this confirmation to the
Campus Wellness Portal, which then displays a \"Cancellation
Confirmation\" message to the Student. If the deletion fails---due to
reasons such as the appointment not being found or being in the
past---the system sends an error message, and the portal displays a
\"Cancellation Failed\" notification. This diagram captures the complete
set of actions, conditions, and system responses associated with the
appointment cancellation functionality.

#### Reschedule Appointment

+---------------------------+------------------+---------------------------------+
| **No.**                   | **Section**      | **Context/Explanation**         |
+:===============+:=========+:=================+:================================+
| **ID**         | 1.1      | Use Case ID      | UC05                            |
|                +----------+------------------+---------------------------------+
|                | 1.2      | Name             | Reschedule Appointment          |
+----------------+----------+------------------+---------------------------------+
| **Management** | 2.1      | Author(s)        | Mohammed Yousef Mohammed        |
|                |          |                  | Abdulkarem                      |
|                +----------+------------------+---------------------------------+
|                | 2.2      | Version          | 1.0                             |
+----------------+----------+------------------+---------------------------------+
| **Context**    | 3.1      | Source(s)        | Questionnaire (Microsoft Forms) |
+----------------+----------+------------------+---------------------------------+
| **Use Case     | 4.1      | Short            | Allows students to change an    |
| Definition**   |          | Description      | existing appointment to a       |
|                |          |                  | different available slot.       |
|                +----------+------------------+---------------------------------+
|                | 4.2      | Associated       | - G1.1 -- CLiC Integration      |
|                |          | Goal(s)          |                                 |
|                |          |                  | - G1.2 -- Manage Appointments   |
|                +----------+------------------+---------------------------------+
|                | 4.3      | Primary Actor(s) | Student                         |
|                +----------+------------------+---------------------------------+
|                | 4.4      | Other Actor(s)   | Admin                           |
|                +----------+------------------+---------------------------------+
|                | 4.5      | Precondition(s)  | - Student is authenticated via  |
|                |          |                  |   the portal.                   |
|                |          |                  |                                 |
|                |          |                  | - At least one valid upcoming   |
|                |          |                  |   appointment exists.           |
|                +----------+------------------+---------------------------------+
|                | 4.6      | Postcondition(s) | - Original appointment is       |
|                |          |                  |   cancelled.                    |
|                |          |                  |                                 |
|                |          |                  | - New appointment is confirmed. |
|                |          |                  |                                 |
|                |          |                  | - Student is notified of the    |
|                |          |                  |   updated appointment.          |
|                +----------+------------------+---------------------------------+
|                | 4.7      | Result           | The system updates the          |
|                |          |                  | appointment to the new selected |
|                |          |                  | date and time, replacing the    |
|                |          |                  | previous schedule, and updates  |
|                |          |                  | its availability on the system. |
|                +----------+------------------+---------------------------------+
|                | 4.8      | Main Scenario    | 1\. Student accesses "My        |
|                |          |                  | Appointments" dashboard.\       |
|                |          |                  | 2. System validates session and |
|                |          |                  | fetches scheduled               |
|                |          |                  | appointments.\                  |
|                |          |                  | 3. Student clicks on            |
|                |          |                  | "Reschedule" button on          |
|                |          |                  | appointment.\                   |
|                |          |                  | 4. System displays updated list |
|                |          |                  | of available slots.\            |
|                |          |                  | 5. Student selects a new        |
|                |          |                  | preferred slot.\                |
|                |          |                  | 6. System validates slot        |
|                |          |                  | availability and checks for     |
|                |          |                  | conflicts.\                     |
|                |          |                  | 7. System performs a            |
|                |          |                  | transaction to cancel the old   |
|                |          |                  | appointment and confirm the new |
|                |          |                  | one.\                           |
|                |          |                  | 8. Notification Service sends   |
|                |          |                  | updated confirmation email.\    |
|                |          |                  | 9. System displays rescheduling |
|                |          |                  | success message.                |
|                +----------+------------------+---------------------------------+
|                | 4.9      | Alternative      | \- 4a. No Suitable Slots        |
|                |          | Scenario(s)      | Available:\                     |
|                |          |                  |  4a1. System displays: "No      |
|                |          |                  | suitable slots found---please   |
|                |          |                  | try again later."\              |
|                |          |                  | - 6a. Time Conflict with        |
|                |          |                  | Another Appointment:\           |
|                |          |                  |  6a1. System prompts student to |
|                |          |                  | select an alternative slot.     |
+----------------+----------+------------------+---------------------------------+

: []{#_Toc199101182 .anchor}Table 4.5 - Reschedule Appointment Use Case

##### Sequence Diagram

<figure>
<img src="media/image12.png" style="width:6.26806in;height:3.39028in"
alt="A diagram of a diagram AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101124" class="anchor"></span>Figure
4.10 - Reschedule Appointment Sequence Diagram</p></figcaption>
</figure>

**Figure 4.10** shows a sequence diagram for the Student rescheduling an
appointment via the Campus Wellness Portal. The Student accesses the
\"My Appointments\" page, triggering session validation by the
Authentication Service. After successful validation, the Student selects
\"Reschedule Appointment.\" The portal requests the current appointment
details from the Medical Center Service, which retrieves them from the
MedicalDB and returns the data. The portal then displays the reschedule
form, and the Student submits a new date and time. If slots are
available, the Medical Center Service updates the appointment in the
MedicalDB, confirms the update to the portal, and the Notification
Service sends a confirmation email. The portal then displays a
confirmation message to the Student. If no slots are available, the
Medical Center Service notifies the portal, which informs the Student
that the selected slot is unavailable and requests a new selection. This
diagram details the sequence of interactions and system decisions in the
rescheduling process.

##### Activity Diagram

<figure>
<img src="media/image13.png" style="width:6.26806in;height:6.19028in"
alt="A diagram of a company AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101125" class="anchor"></span>Figure
4.11 - Reschedule Appointment Activity Diagram</p></figcaption>
</figure>

**Figure 4.11** presents an activity diagram outlining the workflow for
a Student to reschedule an appointment via the Campus Wellness Portal,
involving the Medical Center Service and the Appointment Database. The
process starts with the Student opening the \"My Appointment\" page. The
Campus Wellness Portal requests and displays upcoming appointments by
querying the Medical Center Service, which retrieves data from the
Appointment Database. The Student selects an appointment to reschedule,
prompting the portal to request alternative available slots from the
Medical Center Service. These slots are fetched from the Appointment
Database and displayed to the Student. Upon selecting a new slot, the
Student submits a reschedule request, which the portal forwards to the
Medical Center Service. The Medical Center Service updates the
appointment in the Appointment Database by replacing the old slot with
the new one. The database confirms success or failure, and this status
is returned to the portal. The portal then displays either a
confirmation message for a successful update or an error message if the
update fails, completing the process.

#### View Counselling History

+-----------------------------+------------------+---------------------------------------------------------------------------+
| **No.**                     | **Section**      | **Context/Explanation**                                                   |
+:===============+:===========+:=================+:==========================================================================+
| **ID**         | 1.1        | Use Case ID      | UC06                                                                      |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 1.2        | Name             | View Counselling History                                                  |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Management** | 2.1        | Author(s)        | Farah Hanim binti Mohd Zamri                                              |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 2.2        | Version          | 1.0                                                                       |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Context**    | 3.1        | Source(s)        | Questionnaire (Microsoft Forms)                                           |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Use Case     | 4.1        | Short            |   ----------------------------------------------------------------------- |
| Definition**   |            | Description      |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |                                                                           |
|                |            |                  | The student views their past counselling sessions by selecting a date     |
|                |            |                  | range                                                                     |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.2        | Associated       | - G2.2 -- View Counselling History                                        |
|                |            | Goal(s)          |                                                                           |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.3        | Primary Actor(s) | Student                                                                   |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.4        | Other Actor(s)   | Health Center System, MMU Online Portal                                   |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.5        | Precondition(s)  | - Student must be logged in via SSO                                       |
|                |            |                  |                                                                           |
|                |            |                  | - The system is connected to the counselling database.                    |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.6        | Postcondition(s) | - Student sees a list of past sessions or a message that no records were  |
|                |            |                  |   found.                                                                  |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.7        | Result           | Counselling records are retrieved and displayed based on the selected     |
|                |            |                  | date range.                                                               |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.8        | Main Scenario    | 1.  Student selects "View Counselling History".                           |
|                |            |                  |                                                                           |
|                |            |                  | 2.  System checks authentication.                                         |
|                |            |                  |                                                                           |
|                |            |                  | 3.  System queries counselling records for the selected date range.       |
|                |            |                  |                                                                           |
|                |            |                  | 4.  System displays the results.                                          |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.9        | Alternate        | - No records found: A message is shown.                                   |
|                |            | Scenario(s)      |                                                                           |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.10       | Exception        | - Student is not authenticated: Prompted to log in first.                 |
|                |            | Scenario(s)      |                                                                           |
+----------------+------------+------------------+---------------------------------------------------------------------------+

: []{#_Toc199101183 .anchor}Table 4.6 - View Counselling History Use
Case

##### Sequence Diagram

<figure>
<img src="media/image14.png" style="width:6.26806in;height:4.28958in"
alt="A diagram of a diagram AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101126" class="anchor"></span>Figure
4.12 - View Counselling History Sequence Diagram</p></figcaption>
</figure>

**Figure 4.12** illustrates the sequence diagram by defining the
interaction between the student, user interface, SSO authentication
module, counselling module, and database. The student\'s request is
first validated for authentication. On failure, it shows an error. On
success, the user interface proceeds to fetch the counselling history
data by querying the database through the counselling module. The system
then verifies whether records exist---if yes, it fetches and shows them
to the student; otherwise, it shows an appropriate message. The diagram
includes alternate flows for both authenticated and unauthenticated
users, and for when no records are available, covering all possible
outcomes.

##### Activity Diagram

<figure>
<img src="media/image15.png" style="width:5.13462in;height:4.13568in"
alt="A diagram of a program AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101127" class="anchor"></span>Figure
4.13 - View Counselling History Activity Diagram</p></figcaption>
</figure>

**Figure 4.13** shows the View Counselling Activity Diagram that
illustrates the action a student performs in order to view his/her past
counselling session history through the Campus Wellness Portal. In the
activity diagram, the student initiates use case by selecting \"View
Counselling History\" and a facultative date range. The system validates
whether the student is authenticated by the Single Sign-On (SSO)
service. If the student is not logged in, a prompt is displayed to ask
the student to login. In case of authentication, the system will attempt
to retrieve the counselling records for the entered date range. Based on
whether there are records or not, the system displays the session
details (date, counsellor, and summary) or notifies the student that
there are no records for the chosen date range.

#### View Gym Available Sessions

+---------------------------+------------------+-------------------------------+
| No.                       | Section          | Context/Explanation           |
+:==============+:==========+:=================+:==============================+
| ID            | 1.1       | Use Case ID      | UC07                          |
|               +-----------+------------------+-------------------------------+
|               | 1.2       | Name             | View Gym Available Sessions   |
+---------------+-----------+------------------+-------------------------------+
| Management    | 2.1       | Author(s)        | Mohammed Aamena Mohammed      |
|               |           |                  | Abdulkarem                    |
|               +-----------+------------------+-------------------------------+
|               | 2.2       | Version          | 1.0                           |
+---------------+-----------+------------------+-------------------------------+
| Context       | 3.1       | Source(s)        | Questionnaire (Microsoft      |
|               |           |                  | Forms)                        |
+---------------+-----------+------------------+-------------------------------+
| Use Case      | 4.1       | Short            | Enables a student to view     |
| Definition    |           | Description      | real-time gym session         |
|               |           |                  | availability through the      |
|               |           |                  | Campus Wellness Portal,       |
|               |           |                  | including capacity, timing,   |
|               |           |                  | and gender-specific           |
|               |           |                  | constraints.                  |
|               +-----------+------------------+-------------------------------+
|               | 4.2       | Associated       | - G3.2 -- Gym Schedules       |
|               |           | Goal(s)          |                               |
|               +-----------+------------------+-------------------------------+
|               | 4.3       | Primary Actor(s) | Student                       |
|               +-----------+------------------+-------------------------------+
|               | 4.4       | Other Actor(s)   | Admin                         |
|               +-----------+------------------+-------------------------------+
|               | 4.5       | Precondition(s)  | \- Student is successfully    |
|               |           |                  | authenticated through the     |
|               |           |                  | Campus Wellness Portal.\      |
|               |           |                  | - Gym session data is         |
|               |           |                  | available from backend        |
|               |           |                  | fitness services.             |
|               +-----------+------------------+-------------------------------+
|               | 4.6       | Postcondition(s) | \- Student successfully views |
|               |           |                  | available sessions with       |
|               |           |                  | real-time status and          |
|               |           |                  | constraints.                  |
|               +-----------+------------------+-------------------------------+
|               | 4.7       | Result           | The system displays a list of |
|               |           |                  | available gym sessions with   |
|               |           |                  | date, time, and session type  |
|               |           |                  | details to be viewed by the   |
|               |           |                  | user.                         |
|               +-----------+------------------+-------------------------------+
|               | 4.8       | Main Scenario    | 1\. Student accesses the      |
|               |           |                  | "View Gym Schedule"           |
|               |           |                  | interface.\                   |
|               |           |                  | 2. System validates user      |
|               |           |                  | session via the               |
|               |           |                  | Authentication Service.\      |
|               |           |                  | 3. System retrieves real-time |
|               |           |                  | gym schedule data, including  |
|               |           |                  | session timing, capacity,     |
|               |           |                  | gender restrictions, and      |
|               |           |                  | current availability.\        |
|               |           |                  | 4. System displays the data   |
|               |           |                  | in an organized calendar or   |
|               |           |                  | list format.\                 |
|               |           |                  | 5. Student applies            |
|               |           |                  | filters (e.g., by date,       |
|               |           |                  | gender, session type) to      |
|               |           |                  | narrow down the displayed     |
|               |           |                  | options *(optional)*.\        |
|               |           |                  | 6. System processes the       |
|               |           |                  | filters and retrieves updated |
|               |           |                  | session data.\                |
|               |           |                  | 7. System reviews the         |
|               |           |                  | filtered sessions and         |
|               |           |                  | optionally selects a session  |
|               |           |                  | to book, triggering UC08:     |
|               |           |                  | Book Fitness Class.           |
|               +-----------+------------------+-------------------------------+
|               | 4.9       | Alternative      | - 5a. No Filters Applied\     |
|               |           | Scenario(s)      |    5a1. System defaults to    |
|               |           |                  |   displaying all sessions     |
|               |           |                  |   scheduled within the        |
|               |           |                  |   current week.               |
|               |           |                  |                               |
|               |           |                  | - 6a. No Sessions Available\  |
|               |           |                  |    6a1. System displays: "No  |
|               |           |                  |   available sessions at this  |
|               |           |                  |   time."                      |
|               |           |                  |                               |
|               |           |                  | - 6b. Filtered Results Yield  |
|               |           |                  |   No Matches\                 |
|               |           |                  |    6b1. System displays: "No  |
|               |           |                  |   sessions match your         |
|               |           |                  |   selected criteria. Please   |
|               |           |                  |   adjust filters and try      |
|               |           |                  |   again."                     |
+---------------+-----------+------------------+-------------------------------+

: []{#_Toc199101184 .anchor}Table 4.7 - View Gym Available Sessions Use
Case

##### Sequence Diagram

<figure>
<img src="media/image16.png" style="width:6.26806in;height:3.32986in"
alt="A diagram of a project AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101128" class="anchor"></span>Figure
4.14 - View Gym Available Sessions Sequence Diagram</p></figcaption>
</figure>

**Figure 4.14** presents a sequence diagram that outlines the process
for a Student to view the gym schedule via the Campus Wellness Portal,
involving the Authentication Service, Fitness Center Service, and
FitnessDB. The sequence begins when the Student accesses the \"View Gym
Schedule\" page, prompting the portal to validate the session through
the Authentication Service. Upon successful authentication, the flow
branches based on whether the Student applies filters. If filters are
applied---such as gender or date---the Campus Wellness Portal sends a
filtered session request to the Fitness Center Service, which queries
the FitnessDB and returns the matched sessions. If no filters are
applied, the portal requests the full weekly schedule, and the Fitness
Center Service returns all current sessions from the FitnessDB. In both
cases, the Campus Wellness Portal delivers the resulting session list
and displays the available gym sessions to the Student. The diagram
captures all relevant interactions and system responsibilities for
viewing gym schedules.

##### Activity Diagram

<figure>
<img src="media/image17.png" style="width:6.26806in;height:5.07847in"
alt="A diagram of a workflow AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101129" class="anchor"></span>Figure
4.15 - View Gym Available Sessions Activity Diagram</p></figcaption>
</figure>

**Figure 4.15** presents an activity diagram outlining the workflow for
a Student to view gym sessions through the Campus Wellness Portal,
integrated with the Fitness Center Service and the Fitness Database. The
process begins when the Student selects the \"View Gym Sessions\"
option. The system verifies the user\'s login status; if not
authenticated, the Student is redirected to the login page. Upon
successful login, the portal requests the weekly session data from the
Fitness Center Service, which queries the Fitness Database and returns
the results. If sessions are available, they are displayed to the
Student; otherwise, a \"No sessions available\" message is shown. The
Student may then apply filters such as date or gender. If filters are
applied, the portal sends a filtered request to the Fitness Center
Service, which queries the database and returns any matching sessions.
The portal updates the display accordingly or shows a \"No matching
sessions found\" message if no filtered results are available. This
diagram captures the conditional logic and interactions that ensure
dynamic, filtered access to gym session data.

#### Book Fitness Session

+---------------------------+------------------+---------------------------------+
| **No.**                   | **Section**      | **Context/Explanation**         |
+:===============+:=========+:=================+:================================+
| **ID**         | 1.1      | Use Case ID      | UC08                            |
|                +----------+------------------+---------------------------------+
|                | 1.2      | Name             | Book Fitness Session            |
+----------------+----------+------------------+---------------------------------+
| **Management** | 2.1      | Author(s)        | Mohammed Aamena Mohammed        |
|                |          |                  | Abdulkarem                      |
|                +----------+------------------+---------------------------------+
|                | 2.2      | Version          | 1.0                             |
+----------------+----------+------------------+---------------------------------+
| **Context**    | 3.1      | Source(s)        | Questionnaire (Microsoft Forms) |
+----------------+----------+------------------+---------------------------------+
| **Use Case     | 4.1      | Short            | Allows a student to reserve a   |
| Definition**   |          | Description      | slot in an available fitness    |
|                |          |                  | session through the Campus      |
|                |          |                  | Wellness Portal.                |
|                +----------+------------------+---------------------------------+
|                | 4.2      | Associated       | - G3.1 -- Class Booking         |
|                |          | Goal(s)          |                                 |
|                +----------+------------------+---------------------------------+
|                | 4.3      | Primary Actor(s) | Student                         |
|                +----------+------------------+---------------------------------+
|                | 4.4      | Other Actor(s)   | Admin                           |
|                +----------+------------------+---------------------------------+
|                | 4.5      | Precondition(s)  | \- Student is authenticated via |
|                |          |                  | the Campus Wellness Portal.\    |
|                |          |                  | - Real-time fitness class       |
|                |          |                  | schedule is accessible.         |
|                +----------+------------------+---------------------------------+
|                | 4.6      | Postcondition(s) | \- Success: Student is          |
|                |          |                  | registered for the selected     |
|                |          |                  | session.\                       |
|                |          |                  | - Failure: Student receives     |
|                |          |                  | feedback regarding errors       |
|                |          |                  | (e.g., session full, schedule   |
|                |          |                  | conflict).                      |
|                +----------+------------------+---------------------------------+
|                | 4.7      | Result           | The system confirms and records |
|                |          |                  | the user's booking for the      |
|                |          |                  | selected fitness session and    |
|                |          |                  | updates its availability in the |
|                |          |                  | system.                         |
|                +----------+------------------+---------------------------------+
|                | 4.8      | Main Scenario    | 1\. Student accesses the "Book  |
|                |          |                  | Fitness Class" interface.\      |
|                |          |                  | 2. System displays current      |
|                |          |                  | classes, including time,        |
|                |          |                  | location, and capacity.\        |
|                |          |                  | 3. Student selects a desired    |
|                |          |                  | class.\                         |
|                |          |                  | 4. System checks for            |
|                |          |                  | availability and any scheduling |
|                |          |                  | conflicts.\                     |
|                |          |                  | 5. If valid, system registers   |
|                |          |                  | the student and updates the     |
|                |          |                  | class list.\                    |
|                |          |                  | 6. Notification Service sends a |
|                |          |                  | booking confirmation via        |
|                |          |                  | email.\                         |
|                |          |                  | 7. System displays a success    |
|                |          |                  | message to the student.         |
|                +----------+------------------+---------------------------------+
|                | 4.9      | Alternative      | \- 3a. Class Full:\             |
|                |          | Scenario(s)      |  3a1. System notifies: "Class   |
|                |          |                  | is full -- join waitlist?"\     |
|                |          |                  |  3a2. Student may choose to     |
|                |          |                  | join the waitlist.\             |
|                |          |                  | - 4a. Schedule Conflict:\       |
|                |          |                  |  4a1. System alerts user about  |
|                |          |                  | the conflict with an existing   |
|                |          |                  | booking.                        |
+----------------+----------+------------------+---------------------------------+

: []{#_Toc199101185 .anchor}Table 4.8 - Book Fitness Session Use Case

##### Sequence Diagram

<figure>
<img src="media/image18.png" style="width:6.26806in;height:3.02292in"
alt="A diagram of a class AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101130" class="anchor"></span>Figure
4.16 - Book Fitness Session Sequence Diagram</p></figcaption>
</figure>

**Figure 4.16** presents a sequence diagram detailing the process for a
Student to book a fitness class through the Campus Wellness Portal. The
workflow begins when the Student selects \"Book Fitness
Class\" prompting the portal to validate the login session via the
Authentication Service. Upon successful authentication, the portal
requests available class schedules from the Fitness Center Service,
which queries the Fitness Database and returns a list of upcoming weekly
classes. The Student then selects a class and time slot, and the portal
submits a booking request to the Fitness Center Service. The service
checks slot availability with the Fitness Database. If a slot is
available, the Student is registered, the slot is reserved, and a
confirmation is returned to the portal and emailed to the Student via
the Notification Service. The portal then displays a booking
confirmation message. If the selected class is full, the Fitness Center
Service notifies the portal, which displays a \"Class full!\" message
and offers the Student the option to join a waitlist. This sequence
diagram captures the complete interaction flow and decision points
involved in the fitness class booking process.

##### Activity Diagram

<figure>
<img src="media/image19.png" style="width:6.26806in;height:3.91528in"
alt="A diagram of a company AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101131" class="anchor"></span>Figure
4.17 - Book Fitness Session Activity Diagram</p></figcaption>
</figure>

**Figure 4.17** illustrates the activity diagram for the process of
booking a fitness class through the Campus Wellness Portal. The sequence
begins when the student selects the \"Book Fitness Class\" option. The
system verifies the student\'s login status; if the student is not
authenticated, they are redirected to the login page. Once logged in,
the portal requests available fitness classes from the Fitness Center
Service, which retrieves class schedules and capacity data from the
Fitness Database. If classes are available, the portal displays the list
for the student to select from; otherwise, a \"No classes available\"
message is shown. Upon selecting a desired class, the student submits a
booking request, which the portal forwards to the Fitness Center
Service. The service checks availability in the Fitness Database and, if
a slot is free and there are no conflicts, reserves the slot, sends
confirmation back to the portal, and triggers the Notification Service
to email a booking confirmation to the student. The portal then displays
a \"Booking Successful\" message. If the class is full or a conflict
exists, the request is rejected, and the portal informs the student with
a relevant error message and the option to join a waitlist. This process
ensures efficient interaction and clear communication at each decision
point.

#### Track Wellness Progress

+----------------------------+------------------+-------------------------------+
| **No.**                    | **Section**      | **Context/Explanation**       |
+:===============+:==========+:=================+:==============================+
| **ID**         | 1.1       | Use Case ID      | UC09                          |
|                +-----------+------------------+-------------------------------+
|                | 1.2       | Name             | Track Wellness Progress       |
+----------------+-----------+------------------+-------------------------------+
| **Management** | 2.1       | Author(s)        | Mohammed Aamena Mohammed      |
|                |           |                  | Abdulkarem                    |
|                +-----------+------------------+-------------------------------+
|                | 2.2       | Version          | 1.0                           |
+----------------+-----------+------------------+-------------------------------+
| **Context**    | 3.1       | Source(s)        | Questionnaire (Microsoft      |
|                |           |                  | Forms)                        |
+----------------+-----------+------------------+-------------------------------+
| **Use Case     | 4.1       | Short            | Enables students to monitor   |
| Definition**   |           | Description      | their wellness trends through |
|                |           |                  | interactive dashboards that   |
|                |           |                  | visualize participation,      |
|                |           |                  | goals, and appointments.      |
|                +-----------+------------------+-------------------------------+
|                | 4.2       | Associated       | - G3.3 -- Fitness Tracking    |
|                |           | Goal(s)          |                               |
|                +-----------+------------------+-------------------------------+
|                | 4.3       | Primary Actor(s) | Student                       |
|                +-----------+------------------+-------------------------------+
|                | 4.4       | Other Actor(s)   | Admins                        |
|                +-----------+------------------+-------------------------------+
|                | 4.5       | Precondition(s)  | \- Student is authenticated   |
|                |           |                  | via the Campus Wellness       |
|                |           |                  | Portal.\                      |
|                |           |                  | - System and data sources are |
|                |           |                  | operational and up to date.   |
|                +-----------+------------------+-------------------------------+
|                | 4.6       | Postcondition(s) | \- Student receives a visual  |
|                |           |                  | summary of wellness           |
|                |           |                  | activities and progress.      |
|                +-----------+------------------+-------------------------------+
|                | 4.7       | Result           | The system displays the       |
|                |           |                  | user's wellness data and      |
|                |           |                  | progress over time in a       |
|                |           |                  | clear, summarized format.     |
|                +-----------+------------------+-------------------------------+
|                | 4.8       | Main Scenario    | 1\. Student opens "Track      |
|                |           |                  | Wellness Progress"            |
|                |           |                  | interface.\                   |
|                |           |                  | 2. System validates the       |
|                |           |                  | session.\                     |
|                |           |                  | 3. System retrieves data from |
|                |           |                  | the Medical Centre, Fitness   |
|                |           |                  | Centre, and Wellness Goals    |
|                |           |                  | database.\                    |
|                |           |                  | 4. Analytics Service analyses |
|                |           |                  | trends, achievements, and     |
|                |           |                  | participation.\               |
|                |           |                  | 5. System displays wellness   |
|                |           |                  | insights using charts and     |
|                |           |                  | progress bars.                |
|                +-----------+------------------+-------------------------------+
|                | 4.9       | Alternative      | \- 4a. Milestone Achieved:\   |
|                |           | Scenario(s)      |  4a1. If a milestone is       |
|                |           |                  | achieved, the Notification    |
|                |           |                  | Service sends a motivational  |
|                |           |                  | email message to the student. |
+----------------+-----------+------------------+-------------------------------+

: []{#_Toc199101186 .anchor}Table 4.9 - Track Wellness Progress Use Case

##### Sequence Diagram

<figure>
<img src="media/image20.png" style="width:6.26806in;height:2.87431in"
alt="A screenshot of a diagram AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101132" class="anchor"></span>Figure
4.18 - Track Wellness Progress Sequence Diagram</p></figcaption>
</figure>

**Figure 4.18** presents a sequence diagram that outlines the process by
which a student tracks their wellness progress through the Campus
Wellness Portal, integrating multiple backend services. The process
begins when the student accesses the \"Track Wellness Progress\"
section, prompting the portal to authenticate the session via the
Authentication Service. Upon successful validation, the portal retrieves
data sequentially: weekly fitness activities from the FitnessDB, medical
appointments and counseling session records from the MedicalDB, and
goal-related metrics from the WellnessDB. This aggregated data is then
processed, with support from the Analytics Service, to calculate the
student's overall wellness progress and generate visual performance
summaries. If the system detects that a goal has been achieved, it
triggers the Notification Service to send a congratulatory email and
display a motivational message. The portal concludes by presenting a
detailed progress dashboard to the student, displaying activity trends,
milestones, and goal completion status in a user-friendly interface.

##### Activity Diagram

<figure>
<img src="media/image21.png" style="width:6.26806in;height:2.82569in"
alt="A diagram of a computer AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101133" class="anchor"></span>Figure
4.19 - Track Wellness Progress Activity Diagram</p></figcaption>
</figure>

**Figure 4.19** presents an activity diagram detailing the workflow for
a student to track their wellness progress using the Campus Wellness
Portal, which integrates several backend systems. The process initiates
when the student selects the \"Track Wellness Progress\" feature. The
portal first verifies the user\'s authentication status---redirecting to
the login page if necessary. Upon successful authentication, the portal
retrieves fitness activity data from the Fitness Center System, medical
and counselling data from the Medical Center System, and goal progress
data from the Wellness Database. This data is aggregated and forwarded
to the Analytics Service, which processes the inputs to identify trends,
evaluate goal completion, and generate insights. The system then
displays key wellness indicators---such as charts, KPIs, and progress
levels---on the portal interface. If a wellness goal has been achieved,
the Notification Service is triggered to deliver a motivational message
to the student. This activity diagram illustrates a seamless and
data-driven workflow that empowers students to monitor and celebrate
their wellness achievements.

#### Set Wellness Goals

+----------------------------+------------------+---------------------------------+
| **No.**                    | **Section**      | **Context/Explanation**         |
+:===============+:==========+:=================+:================================+
| **ID**         | 1.1       | Use Case ID      | UC10                            |
|                +-----------+------------------+---------------------------------+
|                | 1.2       | Name             | Set Wellness Goals              |
+----------------+-----------+------------------+---------------------------------+
| **Management** | 2.1       | Author(s)        | Mohammed Aamena Mohammed        |
|                |           |                  | Abdulkarem                      |
|                +-----------+------------------+---------------------------------+
|                | 2.2       | Version          | 1.0                             |
+----------------+-----------+------------------+---------------------------------+
| **Context**    | 3.1       | Source(s)        | Questionnaire (Microsoft Forms) |
+----------------+-----------+------------------+---------------------------------+
| **Use Case     | 4.1       | Short            | Allows students to set and      |
| Definition**   |           | Description      | track personal wellness goals   |
|                |           |                  | such as fitness routines or     |
|                |           |                  | mental health targets.          |
|                +-----------+------------------+---------------------------------+
|                | 4.2       | Associated       | - G4.1 -- Goal Tracking         |
|                |           | Goal(s)          |                                 |
|                +-----------+------------------+---------------------------------+
|                | 4.3       | Primary Actor(s) | Student                         |
|                +-----------+------------------+---------------------------------+
|                | 4.4       | Other Actor(s)   | ---                             |
|                +-----------+------------------+---------------------------------+
|                | 4.5       | Precondition(s)  | \- Student is authenticated and |
|                |           |                  | has access to goal-setting      |
|                |           |                  | functionality.                  |
|                +-----------+------------------+---------------------------------+
|                | 4.6       | Postcondition(s) | \- Success: Goal is saved and   |
|                |           |                  | tracked by the system.\         |
|                |           |                  | - Failure: Input error is       |
|                |           |                  | presented to the student for    |
|                |           |                  | correction.                     |
|                +-----------+------------------+---------------------------------+
|                | 4.7       | Result           | The system saves the user's     |
|                |           |                  | personalized wellness goals and |
|                |           |                  | updates the progress tracking   |
|                |           |                  | accordingly.                    |
|                +-----------+------------------+---------------------------------+
|                | 4.8       | Main Scenario    | 1\. Student navigates to the    |
|                |           |                  | "Set Wellness Goal" interface.\ |
|                |           |                  | 2. System authenticates the     |
|                |           |                  | session.\                       |
|                |           |                  | 3. Student enters goal details, |
|                |           |                  | including activity type (e.g.,  |
|                |           |                  | steps, workout, gym sessions),  |
|                |           |                  | target frequency (e.g., 3       |
|                |           |                  | times/week), and duration       |
|                |           |                  | (e.g., 30 minutes/session).\    |
|                |           |                  | 4. System validates the goal    |
|                |           |                  | format.\                        |
|                |           |                  | 5. System stores the goal in    |
|                |           |                  | the database.\                  |
|                |           |                  | 6. Notification Service sends a |
|                |           |                  | confirmation message.\          |
|                |           |                  | 7. System displays the success  |
|                |           |                  | message and summary.            |
|                +-----------+------------------+---------------------------------+
|                | 4.9       | Alternative      | \- 4a. Invalid Input Format:\   |
|                |           | Scenario(s)      |  4a1. System highlights input   |
|                |           |                  | error and prompts for           |
|                |           |                  | correction.                     |
+----------------+-----------+------------------+---------------------------------+

: []{#_Toc199101187 .anchor}Table 4.10 - Set Wellness Goals Use Case

##### Sequence Diagram

<figure>
<img src="media/image22.png" style="width:6.26806in;height:2.99306in"
alt="A diagram of a company AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101134" class="anchor"></span>Figure
4.20 - Set Wellness Goals Sequence Diagram</p></figcaption>
</figure>

**Figure 4.20** illustrates a sequence diagram representing the process
for a student to set a wellness goal through the Campus Wellness Portal,
involving interactions with the Authentication Service, Goal Management
Service, and WellnessDB. The process begins when the student clicks the
\"Set Wellness Goal\" button, prompting the portal to verify the
student's session via the Authentication Service. Once the session is
confirmed as valid, the student enters goal details---such as target
steps, workouts, or duration---which are then submitted to the Goal
Management Service. This service first validates the format and
completeness of the goal data. If the goal is valid, the system proceeds
to save the data into the WellnessDB, returning a success response to
the portal. The portal then displays a confirmation message and a
summary of the configured goal to the student. Alternatively, if the
submitted goal is invalid---due to missing or incorrect data---a
validation error is returned, and the portal presents an error message
with suggested corrections. This diagram captures both the standard and
alternative flows involved in ensuring robust goal-setting functionality
with real-time feedback.

##### Activity Diagram

<figure>
<img src="media/image23.png" style="width:6.09825in;height:3.57292in"
alt="A diagram of a workflow AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101135" class="anchor"></span>Figure
4.21 - Set Wellness Goals Activity Diagram</p></figcaption>
</figure>

**Figure 4.21** illustrates the activity diagram for the "Set Wellness
Goal" use case in the Campus Wellness Portal. The process begins when
the student selects the "Set Wellness Goal" interface and enters goal
parameters such as goal type, frequency, and duration. The system
verifies the student's session using the Authentication Service. If the
session is invalid, the student is redirected to the login page. If
valid, the system validates the format and content of the goal input. If
the input is invalid, the system returns validation errors and prompts
the student to revise the goal details. Upon successful validation, the
system stores the goal in the Wellness Database and confirms the setup.
A goal summary is displayed to the student, and the Notification Service
issues a confirmation message. This process ensures authenticated
access, proper goal formatting, reliable data storage, and timely
feedback to the user.

#### Get AI Wellness Tips

+-----------------------------+------------------+---------------------------------------------------------------------------+
| **No.**                     | **Section**      | **Context/Explanation**                                                   |
+:===============+:===========+:=================+:==========================================================================+
| **ID**         | 1.1        | Use Case ID      | UC11                                                                      |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 1.2        | Name             | Get AI Wellness Tips                                                      |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Management** | 2.1        | Author(s)        | Nur Thayiebah Binti Hamdan                                                |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 2.2        | Version          | 1.0                                                                       |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Context**    | 3.1        | Source(s)        | Brainstorming (Microsoft Teams), Questionnaire (Microsoft Forms)          |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Use Case     | 4.1        | Short            |   ----------------------------------------------------------------------- |
| Definition**   |            | Description      |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |                                                                           |
|                |            |                  | Provides students with personalized health and wellness tips generated by |
|                |            |                  | an AI engine using their wellness data and activity patterns.             |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.2        | Associated       | - G4.2 AI Tips                                                            |
|                |            | Goal(s)          |                                                                           |
|                |            |                  | - G6.1 Preventive Care                                                    |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.3        | Primary Actor(s) | Student                                                                   |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.4        | Other Actor(s)   | - AI Wellness Engine                                                      |
|                |            |                  |                                                                           |
|                |            |                  | - Wellness Tracking Module                                                |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.5        | Precondition(s)  | - Student is logged in through SSO                                        |
|                |            |                  |                                                                           |
|                |            |                  | - AI tip engine is functional                                             |
|                |            |                  |                                                                           |
|                |            |                  | - Student has a profile or activity data available                        |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.5        | Postcondition(s) | - Student has received one or more tips                                   |
|                |            |                  |                                                                           |
|                |            |                  | - System records interaction (viewed/saved/skipped)                       |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.6        | Result           | Student gains a customized recommendation to improve their health or      |
|                |            |                  | habits.                                                                   |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.7        | Main Scenario    | 1.  Student logs in to the portal.                                        |
|                |            |                  |                                                                           |
|                |            |                  | 2.  Student navigates to the AI Tips section and clicks the "Get Tips"    |
|                |            |                  |     button.                                                               |
|                |            |                  |                                                                           |
|                |            |                  | 3.  The system verifies the session and retrieves the student's wellness  |
|                |            |                  |     data.                                                                 |
|                |            |                  |                                                                           |
|                |            |                  | 4.  If data is sufficient. The AI engine generates personalized wellness  |
|                |            |                  |     tips.                                                                 |
|                |            |                  |                                                                           |
|                |            |                  | 5.  The system displays the tips on the student's dashboard.              |
|                |            |                  |                                                                           |
|                |            |                  | 6.  Student views the tips and may choose to save or dismiss them.        |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.8        | Exception        | - AI Engine Failure:                                                      |
|                |            | Scenario         |                                                                           |
|                |            |                  |   - System fails to generate tips; displays "Tips unavailable" and logs   |
|                |            |                  |     the error.                                                            |
|                |            |                  |                                                                           |
|                |            |                  | - No Wellness Data Available:                                             |
|                |            |                  |                                                                           |
|                |            |                  |   - System prompts student to set wellness goals; may show default        |
|                |            |                  |     advice.                                                               |
+----------------+------------+------------------+---------------------------------------------------------------------------+

: []{#_Toc199101188 .anchor}Table 4.11 - Get AI Wellness Tips Use Case

##### Sequence Diagram

![[]{#_Toc199101136 .anchor}Figure 4.22 - Get AI Wellness Tips Sequence
Diagram](media/image24.jpeg){width="6.268055555555556in"
height="4.183926071741032in"}

**Figure 4.22** illustrates the sequence diagram for the "Get AI
Wellness Tips" use case in the Campus Wellness Portal. The interaction
begins when a student clicks the "Get Tips" button. The system requests
the student's wellness goals and activity data from the Wellness Data
Service. If data is available, it is forwarded to the AI Wellness Engine
to generate a personalized wellness tip, which is then displayed to the
student. The student may choose to save or dismiss the tip. If no data
is found, the system prompts the student to set their wellness goals
first. This ensures that tips are tailored and relevant to each user's
wellness journey.

##### Activity Diagram

<figure>
<img src="media/image25.png" style="width:4.875in;height:5.08186in"
alt="A screenshot of a computer AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101137" class="anchor"></span>Figure
4.23 - Get AI Wellness Tips Activity Diagram</p></figcaption>
</figure>

**Figure 4.23** illustrates the activity diagram for the "Get AI
Wellness Tips" use case in the Campus Wellness Portal. The process
begins when the student logs into the system via MMU's Single Sign-On
(SSO). Once authenticated, the student navigates to the AI Tips section
and clicks the "Get Tips" button. The system retrieves the student's
wellness data and checks for completeness. If the data is insufficient
--- for example, if no goals have been set --- the system displays a
message prompting the student to configure their goals. If sufficient
data is available, the system invokes the AI Engine to generate a
personalized tip. If the generation is successful, the tip is displayed
to the student. If the AI fails to generate a tip, an error message is
shown instead. The student then has the option to either save the tip or
exit the interface.

#### Receive Notification

+-----------------------------+------------------+--------------------------------+
| **No.**                     | **Section**      | **Context/Explanation**        |
+:===============+:===========+:=================+:===============================+
| **ID**         | 1.1        | Use Case ID      | UC12                           |
|                +------------+------------------+--------------------------------+
|                | 1.2        | Name             | Receive Notification           |
+----------------+------------+------------------+--------------------------------+
| **Management** | 2.1        | Author(s)        | Nur Thayiebah Binti Hamdan     |
|                +------------+------------------+--------------------------------+
|                | 2.2        | Version          | 1.0                            |
+----------------+------------+------------------+--------------------------------+
| **Context**    | 3.1        | Source(s)        | Questionnaire (Microsoft       |
|                |            |                  | Forms)                         |
+----------------+------------+------------------+--------------------------------+
| **Use Case     | 4.1        | Short            | Enables the system to deliver  |
| Definition**   |            | Description      | time-sensitive notifications   |
|                |            |                  | to students about their        |
|                |            |                  | upcoming appointments,         |
|                |            |                  | sessions, or health            |
|                |            |                  | activities.                    |
|                +------------+------------------+--------------------------------+
|                | 4.2        | Associated       | - G1.3 Reminders,              |
|                |            | Goal(s)          |                                |
|                |            |                  | - G6.3 Promote Usage           |
|                +------------+------------------+--------------------------------+
|                | 4.3        | Primary Actor(s) | Student                        |
|                +------------+------------------+--------------------------------+
|                | 4.4        | Other Actor(s)   | - Notification Engine          |
|                |            |                  |                                |
|                |            |                  | - Campus Wellness Scheduler    |
|                +------------+------------------+--------------------------------+
|                | 4.5        | Precondition(s)  | - Student has scheduled events |
|                |            |                  |   in the system                |
|                |            |                  |                                |
|                |            |                  | - notification settings are    |
|                |            |                  |   enabled for the student      |
|                |            |                  |                                |
|                |            |                  | - background notification job  |
|                |            |                  |   is running                   |
|                +------------+------------------+--------------------------------+
|                | 4.5        | Postcondition(s) | - Student receives and views   |
|                |            |                  |   the notification             |
|                |            |                  |                                |
|                |            |                  | - Student may act upon the     |
|                |            |                  |   notification or dismiss it   |
|                +------------+------------------+--------------------------------+
|                | 4.6        | Result           | Students are reminded of       |
|                |            |                  | important events and prompted  |
|                |            |                  | to take timely actions (e.g.,  |
|                |            |                  | attend reschedule)             |
|                +------------+------------------+--------------------------------+
|                | 4.7        | Main Scenario    | 1.  Student initiates a        |
|                |            |                  |     scheduled background job   |
|                |            |                  |     to check upcoming student  |
|                |            |                  |     events.                    |
|                |            |                  |                                |
|                |            |                  | 2.  System checks if there are |
|                |            |                  |     any events scheduled for   |
|                |            |                  |     each student.              |
|                |            |                  |                                |
|                |            |                  | 3.  If upcoming events exist,  |
|                |            |                  |     the system checks if the   |
|                |            |                  |     student has notifications  |
|                |            |                  |     enabled.                   |
|                |            |                  |                                |
|                |            |                  | 4.  If enabled, the system     |
|                |            |                  |     generates the notification |
|                |            |                  |     content.                   |
|                |            |                  |                                |
|                |            |                  | 5.  System sends the           |
|                |            |                  |     notification to the        |
|                |            |                  |     student.                   |
|                |            |                  |                                |
|                |            |                  | 6.  Student receives the       |
|                |            |                  |     notification.              |
|                |            |                  |                                |
|                |            |                  | 7.  Student views the          |
|                |            |                  |     notification.              |
|                |            |                  |                                |
|                |            |                  | 8.  Student chooses to either  |
|                |            |                  |     take action (e.g., open    |
|                |            |                  |     schedule, reschedule,      |
|                |            |                  |     cancel) or dismiss the     |
|                |            |                  |     notification.              |
|                +------------+------------------+--------------------------------+
|                | 4.8        | Exception        | - No upcoming events:          |
|                |            | Scenario         |                                |
|                |            |                  |   - System finds no upcoming   |
|                |            |                  |     events; no notification is |
|                |            |                  |     generated.                 |
|                |            |                  |                                |
|                |            |                  | - Notifications disabled       |
|                |            |                  |                                |
|                |            |                  |   - Even if events exist, the  |
|                |            |                  |     system detects that the    |
|                |            |                  |     student has disabled       |
|                |            |                  |     notifications and ends the |
|                |            |                  |     process.                   |
|                |            |                  |                                |
|                |            |                  | - Delivery failure             |
|                |            |                  |                                |
|                |            |                  |   - System fails to send       |
|                |            |                  |     notification (e.g.,        |
|                |            |                  |     network or queue error);   |
|                |            |                  |     message is logged for      |
|                |            |                  |     retry or admin alert.      |
+----------------+------------+------------------+--------------------------------+

: []{#_Toc199101189 .anchor}Table 4.12 - Receive Notification Use Case

##### Sequence Diagram

![[]{#_Toc199101138 .anchor}Figure 4.24 - Receive Notification Sequence
Diagram](media/image26.jpeg){width="3.9529549431321085in"
height="8.870588363954505in"}

**Figure 4.24** illustrates the sequence diagram for the "Receive
Notification" use case in the Campus Wellness Portal. The process is
initiated by the system Scheduler, which triggers a background
notification job. The Notification Service checks for upcoming
student-specific events. If no events are found, the process terminates.
If relevant events exist, the system checks whether notifications are
enabled for the respective student. If notifications are active, the
system generates a personalized message and sends it. The student
receives and views the notification. Depending on its content, the
student may choose to take further action---such as opening the portal
to reschedule or cancel an event---or dismiss it entirely. If
notifications are disabled or message delivery fails, the process is
logged or skipped to prevent unnecessary disruption. This sequence
ensures timely, relevant, and personalized communication with students.

##### Activity Diagram

<figure>
<img src="media/image27.png" style="width:6.26806in;height:5.03333in"
alt="A screenshot of a computer AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101139" class="anchor"></span>Figure
4.25 - Receive Notification Activity Diagram</p></figcaption>
</figure>

**Figure 4.25** illustrates the activity diagram for the "Receive
Notification" use case in the Campus Wellness Portal. The process begins
when the system triggers a daily notification job to check for upcoming
student events. If no events are found, the process ends. If events are
detected, the system verifies whether notifications are enabled for the
corresponding student. If enabled, it generates the notification content
and sends it to the student. Upon receiving the notification, the
student views it and decides whether to act. If the student chooses to
act, they are redirected to the scheduling interface to open,
reschedule, or cancel the event. If no action is taken, the student
dismisses the notification. This activity flow ensures that only
students with valid upcoming events and enabled preferences receive
timely and actionable notifications.

#### Manage Notification

+-----------------------------+------------------+---------------------------------------------------------------------------+
| **No.**                     | **Section**      | **Context/Explanation**                                                   |
+:===============+:===========+:=================+:==========================================================================+
| **ID**         | 1.1        | Use Case ID      | UC13                                                                      |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 1.2        | Name             | Manage Notification                                                       |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Management** | 2.1        | Author(s)        | Nur Thayiebah Binti Hamdan                                                |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 2.2        | Version          | 1.0                                                                       |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Context**    | 3.1        | Source(s)        | Brainstorming (Microsoft Teams), Observation                              |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Use Case     | 4.1        | Short            |   ----------------------------------------------------------------------- |
| Definition**   |            | Description      |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |                                                                           |
|                |            |                  | Allows students to view and update their notification preferences, such   |
|                |            |                  | as toggling appointment reminders or AI health tips, to personalize their |
|                |            |                  | portal experience.                                                        |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.2        | Associated       | - G6.3 Promote Usage                                                      |
|                |            | Goal(s)          |                                                                           |
|                |            |                  | - G5.3 User-Friendly Interface                                            |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.3        | Primary Actor(s) | Student                                                                   |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.4        | Other Actor(s)   | Notification Preferences Manager (System component)                       |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.5        | Precondition(s)  | - Student is logged in via MMU SSO                                        |
|                |            |                  |                                                                           |
|                |            |                  | - Notification settings are already initialized for the student account   |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.5        | Postcondition(s) | - Notification preferences are updated and stored in the database         |
|                |            |                  |                                                                           |
|                |            |                  | - Confirmation is sent to the student                                     |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.6        | Result           | Student customizes their notification experience to match personal        |
|                |            |                  | preferences.                                                              |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.7        | Main Scenario    | 1.  Student logs into the portal via MMU SSO.                             |
|                |            |                  |                                                                           |
|                |            |                  | 2.  System authenticated the student session.                             |
|                |            |                  |                                                                           |
|                |            |                  | 3.  Student navigates to the Notification Settings page.                  |
|                |            |                  |                                                                           |
|                |            |                  | 4.  System fetches current notification preferences and displays them.    |
|                |            |                  |                                                                           |
|                |            |                  | 5.  Student views existing preferences.                                   |
|                |            |                  |                                                                           |
|                |            |                  | 6.  Student decides to modify preferences.                                |
|                |            |                  |                                                                           |
|                |            |                  | 7.  Student submits the updated preferences.                              |
|                |            |                  |                                                                           |
|                |            |                  | 8.  System validates the input.                                           |
|                |            |                  |                                                                           |
|                |            |                  | 9.  If valid, preferences are saved to the database.                      |
|                |            |                  |                                                                           |
|                |            |                  | 10. System sends a confirmation message.                                  |
|                |            |                  |                                                                           |
|                |            |                  | 11. Student sees the confirmation.                                        |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.8        | Exception        | - Invalid input:                                                          |
|                |            | Scenario         |                                                                           |
|                |            |                  |   - If submitted preferences are invalid (e.g., incorrect format), the    |
|                |            |                  |     system shows an error message and prompts the student to correct it.  |
|                |            |                  |                                                                           |
|                |            |                  | - No Changes Made:                                                        |
|                |            |                  |                                                                           |
|                |            |                  |   - If the student chooses not to modify preferences, the session ends    |
|                |            |                  |     without updates.                                                      |
+----------------+------------+------------------+---------------------------------------------------------------------------+

: []{#_Toc199101190 .anchor}Table 4.13 - Manage Notification Use Case

##### Sequence Diagram

![[]{#_Toc199101140 .anchor}Figure 4.26 - Manage Notification Sequence
Diagram](media/image28.jpeg){width="6.257070209973754in"
height="6.810416666666667in"}

**Figure 4.26** illustrates the sequence diagram for the "Manage
Notification" use case in the Campus Wellness Portal. The process begins
when the student logs in via MMU's Single Sign-On (SSO). The system
verifies the session with the Authentication Service. Once
authenticated, the student navigates to the Notification Settings page.
The portal then fetches the current notification preferences by
requesting them from the Notification Service, which retrieves them from
the Preferences Database. After the preferences are displayed, the
student may choose to submit updated preferences. The system validates
the input and, if valid, saves the new settings to the database and
returns a confirmation message. If the input is invalid, an error
message is shown, and the student is prompted to revise the form. If no
changes are submitted, the session concludes without updates. This
process ensures students can personalize how they receive wellness
notifications.

##### Activity Diagram

<figure>
<img src="media/image29.png" style="width:5.23333in;height:5.93722in"
alt="A black background with white text AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101141" class="anchor"></span>Figure
4.27 - Manage Notification Activity Diagram</p></figcaption>
</figure>

**Figure 4.27** illustrates the activity diagram for the "Manage
Notification" use case in the Campus Wellness Portal. The activity
begins when the student logs in via MMU Single Sign-On. The system
authenticates the session and allows the student to access the
Notification Settings interface. The portal retrieves and displays the
student's current notification preferences. The student may then choose
to update their preferences. If no changes are made, the process ends
without modification. If the student submits updated preferences, the
system validates the input. If the input is valid, the preferences are
saved to the database, and a confirmation message is displayed. The
student then views the confirmation. If the input is invalid, the system
presents an error message and prompts the student to correct their
submission. This workflow ensures secure, accurate, and user-driven
management of notification preferences.

#### View Student Wellness Report

+-----------------------------+------------------+---------------------------------------------------------------------------+
| **No.**                     | **Section**      | **Context/Explanation**                                                   |
+:===============+:===========+:=================+:==========================================================================+
| **ID**         | 1.1        | Use Case ID      | UC14                                                                      |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 1.2        | Name             | View Student Wellness Report                                              |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Management** | 2.1        | Author(s)        | Farah Hanim binti Mohd Zamri                                              |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 2.2        | Version          | 1.0                                                                       |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Context**    | 3.1        | Source(s)        | Brainstorming (Microsoft Teams), Observation                              |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Use Case     | 4.1        | Short            |   ----------------------------------------------------------------------- |
| Definition**   |            | Description      |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |                                                                           |
|                |            |                  | The Admin views the wellness records of a student based on a specified    |
|                |            |                  | date range.                                                               |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.2        | Associated       | - G4.3 -- Dashboard                                                       |
|                |            | Goal(s)          |                                                                           |
|                |            |                  | - G6.1 -- Preventive Care                                                 |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.3        | Primary Actor(s) | Student                                                                   |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.4        | Other Actor(s)   | Health Center System, MMU Online Portal                                   |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.5        | Precondition(s)  | - Admin must be logged in via SSO                                         |
|                |            |                  |                                                                           |
|                |            |                  | - Student ID and date range must be specified.                            |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.6        | Postcondition(s) | - Wellness report is displayed OR                                         |
|                |            |                  |                                                                           |
|                |            |                  | - Message: "No records available" is shown                                |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.7        | Result           | Student name, metrics, and summary are displayed if records exist         |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.8        | Main Scenario    | 1.  Admin selects "View Student Wellness Report".                         |
|                |            |                  |                                                                           |
|                |            |                  | 2.  Admin inputs Student ID and date range.                               |
|                |            |                  |                                                                           |
|                |            |                  | 3.  System authenticates admin.                                           |
|                |            |                  |                                                                           |
|                |            |                  | 4.  Wellness report is retrieved and displayed if available.              |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.9        | Alternate        | - If no records are found, system displays "No Wellness Records           |
|                |            | Scenario(s)      |   Available".                                                             |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.10       | Exception        | - If not logged in: System displays "You must be logged in as Admin"      |
|                |            | Scenario(s)      |   error.                                                                  |
+----------------+------------+------------------+---------------------------------------------------------------------------+

: []{#_Toc199101191 .anchor}Table 4.14 - View Student Wellness Report
Use Case

##### Sequence Diagram

<figure>
<img src="media/image30.png" style="width:6.26806in;height:3.83194in"
alt="A diagram of a computer program AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101142" class="anchor"></span>Figure
4.28 - View Student Wellness Report Sequence Diagram</p></figcaption>
</figure>

**Figure 4.28** is the sequence diagram that shows the sequential system
component communication in which an admin is viewing a student wellness
report view. This process starts with the admin requesting it by
selecting the report function and entering a student ID and date range.
The User Interface sends an authentication request via the SSO
Authentication Module. On success, the system proceeds to send a request
to the Wellness Module, which then requests the database for matching
records. The database returns the records (if any) to the Wellness
Module, and the module displays the report with student name, metrics,
and summary or the no records found message. If the admin is
unauthenticated, the system immediately rejects the process and displays
an error message for login. Conditional flows are illustrated through
alt blocks to control record availability and authentication results to
make the diagram understandable in displaying both successful and failed
lines.

##### Activity Diagram

<figure>
<img src="media/image31.png" style="width:6.26806in;height:4.75694in"
alt="A diagram of a program AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101143" class="anchor"></span>Figure
4.29 - View Student Wellness Report Activity Diagram</p></figcaption>
</figure>

**Figure 4.29** is the activity diagram showing the logical flow of an
admin to view a student\'s wellness report through the Campus Wellness
Portal. It is where it begins when the admin selects the \"View Student
Wellness Report\" from the menu. The admin inputs the student\'s ID or
name and the needed date range and clicks on \"Generate Report.\" The
system checks whether the admin is SSO authenticated. If admin is not
logged in, it shows an error message to log in. If logged in, the system
proceeds further to retrieve the wellness data of the student. The
system checks whether records for the specified student and date range
are saved or not. If records have been saved, the student's name,
wellness measures, and summary report is shown. Otherwise, it will give
a message that no records exist for the given parameters.

#### Manage Fitness Class

+-----------------------------+------------------+---------------------------------------------------------------------------+
| **No.**                     | **Section**      | **Context/Explanation**                                                   |
+:===============+:===========+:=================+:==========================================================================+
| **ID**         | 1.1        | Use Case ID      | UC15                                                                      |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 1.2        | Name             | Manage Fitness Class                                                      |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Management** | 2.1        | Author(s)        | Farah Hanim binti Mohd Zamri                                              |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 2.2        | Version          | 1.0                                                                       |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Context**    | 3.1        | Source(s)        | Observation                                                               |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Use Case     | 4.1        | Short            |   ----------------------------------------------------------------------- |
| Definition**   |            | Description      |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |                                                                           |
|                |            |                  | Enables the Admin to add, edit, or remove fitness classes from the        |
|                |            |                  | schedule.                                                                 |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.2        | Associated       | - G6.2 -- Administrative Efficiency                                       |
|                |            | Goal(s)          |                                                                           |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.3        | Primary Actor(s) | Admin                                                                     |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.4        | Other Actor(s)   | Fitness Center System, MMU Online Portal                                  |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.5        | Precondition(s)  | - Admin must be authenticated via SSO                                     |
|                |            |                  |                                                                           |
|                |            |                  | - Admin must have access to class management.                             |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.6        | Postcondition(s) | - Class data is added, updated, or deleted in the system.                 |
|                |            |                  |                                                                           |
|                |            |                  | - Success or error message is shown.                                      |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.7        | Result           | Counselling records are retrieved and displayed based on the selected     |
|                |            |                  | date range.                                                               |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.8        | Main Scenario    | 1.  Admin selects "Manage Fitness Class".                                 |
|                |            |                  |                                                                           |
|                |            |                  | 2.  Admin chooses to add/edit/delete class.                               |
|                |            |                  |                                                                           |
|                |            |                  | 3.  Admin fills/modifies class details.                                   |
|                |            |                  |                                                                           |
|                |            |                  | 4.  System updates class database.                                        |
|                |            |                  |                                                                           |
|                |            |                  | 5.  Success message is shown.                                             |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.9        | Alternate        | - Admin cancels the operation.                                            |
|                |            | Scenario(s)      |                                                                           |
|                |            |                  | - Class data validation fails.                                            |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.10       | Exception        | - SSO Authentication fails: "Login Required" message.                     |
|                |            | Scenario(s)      |                                                                           |
|                |            |                  | - Backend update fails: "Unable to process request. Please try again."    |
+----------------+------------+------------------+---------------------------------------------------------------------------+

: []{#_Toc199101192 .anchor}Table 4.15 - Manage Fitness Class Use Case

##### Sequence Diagram

<figure>
<img src="media/image32.png" style="width:6.26806in;height:5.10069in"
alt="A diagram with text and images AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101144" class="anchor"></span>Figure
4.30 - Manage Fitness Class Sequence Diagram</p></figcaption>
</figure>

**Figure 4.30** outlines the step-by-step interaction needed in managing
fitness classes. It starts with the Admin initiating the management
request via the user interface. The system first checks if the Admin is
authenticated via the SSO Authentication Module. When authentication
fails, it shows an error message. When authenticated, the Admin can add,
edit, or delete a class. The action is relayed to the Fitness Class
Module, which interacts with the database to execute the insert, update,
or delete operation. The system returns success or
failure. The corresponding messages, for instance, \"Class Successfully
Added,\" \"Updated,\" or \"Removed,\" are then shown to the Admin based
on the outcome.

##### Activity Diagram

<figure>
<img src="media/image33.png" style="width:6.26806in;height:3.57569in"
alt="A diagram of a company AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101145" class="anchor"></span>Figure
4.31 - Manage Fitness Class Activity Diagram</p></figcaption>
</figure>

**Figure 4.31** illustrates how an Admin is managing fitness class
records in the Campus Wellness Portal. The process begins when the Admin
selects the \"Manage Fitness Class\" menu option. The Admin
then determines whether they need to add, edit, or delete a
class. To add, the Admin enters class details and clicks \"Add
Class.\" To edit, they change the existing class and click \"Save
Changes.\" To delete, the Admin selects the class and clicks \"Delete
Class.\" Each of these sends a request to the Campus Wellness Portal.
The portal checks if the Admin is authenticated via SSO. If not, it
shows an error message. If the authentication is successful, the
portal performs the request. Depending on the success of the operation,
a confirmation message is displayed, or an error is returned if the
operation fails.

#### Manage Medical Schedule 

+-----------------------------+------------------+---------------------------------------------------------------------------+
| **No.**                     | **Section**      | **Context/Explanation**                                                   |
+:===============+:===========+:=================+:==========================================================================+
| **ID**         | 1.1        | Use Case ID      | UC16                                                                      |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 1.2        | Name             | Manage Medical Schedule                                                   |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Management** | 2.1        | Author(s)        | Nur Thayiebah Binti Hamdan                                                |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 2.2        | Version          | 1.0                                                                       |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Context**    | 3.1        | Source(s)        | Observation                                                               |
+----------------+------------+------------------+---------------------------------------------------------------------------+
| **Use Case     | 4.1        | Short            |   ----------------------------------------------------------------------- |
| Definition**   |            | Description      |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |                                                                           |
|                |            |                  |   ----------------------------------------------------------------------- |
|                |            |                  |                                                                           |
|                |            |                  | Allow staff to add, edit, or remove medical appointment slots through the |
|                |            |                  | Campus Wellness Portal, enabling better control over medical availability |
|                |            |                  | scheduling.                                                               |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.2        | Associated       | - G6.2 Administrative Efficiency                                          |
|                |            | Goal(s)          |                                                                           |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.3        | Primary Actor(s) | Staff                                                                     |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.4        | Other Actor(s)   | Medical Scheduling System                                                 |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.5        | Precondition(s)  | - Staff is logged in through MMU SSO                                      |
|                |            |                  |                                                                           |
|                |            |                  | - Medical schedule data is available in the system                        |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.5        | Postcondition(s) | - Schedule updates are saved and confirmed                                |
|                |            |                  |                                                                           |
|                |            |                  | - Confirmation is sent to the staff interface                             |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.6        | Result           | Medical appointment slots are accurately updated for student booking.     |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.7        | Main Scenario    | 1.  Staff logs into the portal via MMU SSO.                               |
|                |            |                  |                                                                           |
|                |            |                  | 2.  System verifies the staff session.                                    |
|                |            |                  |                                                                           |
|                |            |                  | 3.  Staff navigates to the Medical Schedule Module.                       |
|                |            |                  |                                                                           |
|                |            |                  | 4.  System fetches and displays the current schedule.                     |
|                |            |                  |                                                                           |
|                |            |                  | 5.  Staff chooses to add, edit, or delete an appointment slot.            |
|                |            |                  |                                                                           |
|                |            |                  | 6.  Staff enters or updates the slot details.                             |
|                |            |                  |                                                                           |
|                |            |                  | 7.  System validates the submitted input.                                 |
|                |            |                  |                                                                           |
|                |            |                  | 8.  If input is valid, the system attempts to update the schedule in the  |
|                |            |                  |     database.                                                             |
|                |            |                  |                                                                           |
|                |            |                  | 9.  If update is successful, system sends a confirmation message.         |
|                |            |                  |                                                                           |
|                |            |                  | 10. Staff sees the confirmation message.                                  |
|                +------------+------------------+---------------------------------------------------------------------------+
|                | 4.8        | Exception        | - Invalid Input:                                                          |
|                |            | Scenario         |                                                                           |
|                |            |                  |   - System detects errors (e.g., missing date/time) in the slot details   |
|                |            |                  |     and prompts staff to correct them.                                    |
|                |            |                  |                                                                           |
|                |            |                  | - Update failure:                                                         |
|                |            |                  |                                                                           |
|                |            |                  |   - Database fails to apply the changes (e.g., due to system error);      |
|                |            |                  |     system displays error message and returns staff to input form.        |
+----------------+------------+------------------+---------------------------------------------------------------------------+

: []{#_Toc199101193 .anchor}Table 4.16 - Manage Medical Schedule Use
Case

##### Sequence Diagram

![[]{#_Toc199101146 .anchor}Figure 4.32 - Manage Medical Schedule
Sequence Diagram](media/image34.jpeg){width="6.264818460192476in"
height="8.465972222222222in"}

**Figure 4.32** illustrates the sequence diagram for the "Manage Medical
Schedule" use case in the Campus Wellness Portal. The process begins
when a staff member logs into the portal via MMU Single Sign-On. The
system verifies the session through the Authentication Service. Once
authenticated, the staff navigates to the Medical Schedule Module. The
portal requests and displays the current appointment schedule, which is
retrieved from the Schedule Database via the ScheduleService. The staff
may then submit updates by adding, editing, or removing time slots. The
system validates the input. If the data is valid, the system attempts to
update the database. A confirmation message is sent back to the staff
upon successful update. If the input is invalid or the database update
fails, the system displays an appropriate error message and prompts the
staff to retry or correct the input. This ensures secure, real-time
management of medical schedules.

##### Activity Diagram

<figure>
<img src="media/image35.png" style="width:5.38542in;height:6.1211in"
alt="A black background with white dots AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101147" class="anchor"></span>Figure
4.33 - Manage Medical Schedule Activity Diagram</p></figcaption>
</figure>

**Figure 4.33** illustrates the activity diagram for the "Manage Medical
Schedule" use case.\
The process begins when a staff member logs into the portal, and the
system authenticates the session. After accessing the Medical Schedule
Module, the current schedule is displayed. The staff chooses to modify
an appointment slot and submits the updated slot details. The system
validates the input format and content. If the input is invalid --- for
example, missing date or time --- the system presents an error message
and prompts the staff to correct the entry. If valid, the system
attempts to save the updated schedule. If the update operation is
successful, a confirmation message is shown to the staff. If a system
error occurs and the database fails to process the update, an error is
shown, and the staff is returned to the form to retry. This flow ensures
staff can reliably manage scheduling tasks while maintaining input
accuracy and system integrity.

## Interface Requirements 

> This section outlines the key interfaces that enable interaction
> between the Campus Wellness Portal and its users, external systems,
> and internal modules. All interfaces shall comply with MMU's IT
> policies, Malaysia PDPA, and where applicable, international
> regulations such as GDPR. Interfaces are classified as System
> Interfaces, User Interfaces, Hardware Interfaces, Software Interfaces,
> and Communication Interfaces.

### System Interfaces

- The portal integrates with the University Authentication System
  (LDAP/SSO) for secure single sign-on access, with expected
  authentication completed within 2 seconds.

- The Student Information System (SIS) is used to retrieve enrolment
  status and insurance eligibility details, with synchronization
  expected within 10 seconds.

- The Medical Appointment System supplies real-time data on available
  medical slots and appointment statuses, refreshed every 5 minutes.

- The Fitness Centre Schedule System provides session availability,
  capacity limits, and gender-specific access details, updated every 5
  minutes.

- Integration with Calendar APIs (e.g., Google Calendar, Microsoft
  Outlook) enables users to sync booked appointments, with updates
  reflected within 30 seconds of booking confirmation.

### User Interfaces

- A fully responsive interface supports consistent user experiences
  across mobile devices, tablets, and desktop platforms, ensuring equal
  access to all core functionalities.

- A unified dashboard consolidates features including upcoming
  appointments, wellness goals, and AI-generated tips. It includes a
  fixed top navigation bar (Home, Bookings, Progress, Settings).

- Real-time appointment booking workflows are optimized as follows:

  - **Booking**: Maximum of **3 steps **to schedule an appointment
    (select service → choose slot → confirm).

  - **Slot Display**: Dynamic, real-time listings with **color-coded
    indicators** (e.g., green = available, red = full).

- The user interface adheres to WCAG 2.1 Level AA accessibility
  standards, ensuring inclusivity for users with visual or motor
  impairments.

### Hardware Interfaces

- The system supports integration with wearable fitness devices (e.g.,
  Fitbit, Apple Health) via Bluetooth/Wi-Fi, allowing health data sync
  for progress tracking.

- The architecture is future-ready for optional biometric hardware
  integration (e.g., fingerprint or facial recognition) to enhance
  security for clinical modules.

### Software Interfaces

- A secure cloud storage service will store generated reports, wellness
  records, and user-submitted feedback.

- An AI/ML recommendation engine will analyze health and counselling
  data using natural language processing to generate customized health
  tips.

- The internal notification module sends reminders and confirmation
  messages through SMS and email based on user preferences.

- The portal connects to a Gym Management System, which manages slot
  filtering by gender, updates capacity in real-time, and provides
  feedback integration.

### Communication Interfaces

- **Protocols**:

  - All communications between the client and server use **HTTPS over
    TLS** to ensure encryption and secure data transmission.

  - **RESTful APIs** using JSON are employed for standardized data
    exchange between system modules and third-party services.

- **Message Formats**:

  - **Appointment Notifications** use predefined templates, e.g., "Your
    gym session is confirmed for \[date\] at \[time\]."

  - **Error Messages** are clear and contextual, e.g., "Slot
    unavailable. Please refresh or try again."

- **Network Requirements**:

  - A **minimum bandwidth of 10 Mbps** is required to support real-time
    interactions.

  - In case of limited connectivity, the system supports a **fallback
    offline mode**, which provides access to previously cached booking
    history and schedules.

## Performance Requirements

> The system shall meet the following performance goals to ensure
> responsiveness, scalability, and real-time interaction quality under
> academic load conditions:

  ----------------------------------------------------------------------------
  **ID**   **Performance     **Description**
           Requirement**     
  -------- ----------------- -------------------------------------------------
  PR-01    **System Response The system shall respond to 95% of user actions
           Time**            (e.g., booking, viewing data) within 2 seconds
                             under normal load conditions.

  PR-02    **Concurrent      The system shall support at least 300 concurrent
           Users**           users without performance degradation during peak
                             hours (e.g., enrolment and registration periods).

  PR-03    **Real-time       Availability data for medical slots and gym
           Updates**         sessions shall be refreshed every 5 minutes to
                             ensure accurate user-facing information.

  PR-04    **Notification    Confirmation emails and SMS notifications shall
           Latency**         be dispatched within 30 seconds of completing
                             booking, rescheduling, or cancellation
                             operations.

  PR-05    **Scalability**   The system architecture shall be scalable to
                             support a projected 20% annual increase in
                             concurrent users and transactions without
                             requiring full system redesign.
  ----------------------------------------------------------------------------

  : []{#_Toc199101194 .anchor}Table 4.17 - Performance Requirements

**Reliability and Availability Requirements**

- The system shall offer 99.5% uptime during standard academic operating
  hours (8:00 AM to 10:00 PM, Monday--Saturday).

- The system shall implement automated failover and daily incremental
  backups.

- The system shall support full recovery within 5 minutes following a
  disruption, verified via recovery time objective (RTO) benchmarks.

## Maintainability and Portability Requirements

- The software shall adopt a modular MVC architecture to support easy
  enhancement and debugging.

- The source code shall follow PEP-8 Python style and ReactJS best
  practices for clean and maintainable source.

- The system shall be operable on both Linux and Windows-based servers
  without significant reconfiguration.

## Usability Requirements

> These requirements define the system's ease of use, accessibility, and
> user support capabilities. Usability expectations are guided by ISO
> 9241-210 for user-centred design and WCAG 2.1 Level AA for digital
> accessibility compliance. All key features must be accessible within a
> minimal interaction path (ideally 3 steps) and provide inclusive
> interaction experiences for diverse users.

  --------------------------------------------------------------------------
  **ID**   **Usability        **Description**
           Requirement**      
  -------- ------------------ ----------------------------------------------
  UR-01    **Minimal          All primary user tasks (e.g., booking an
           Navigation Steps** appointment, viewing sessions) shall be
                              achievable within 3 clicks from the dashboard.

  UR-02    **Accessible       The system shall comply with WCAG 2.1 Level
           Interface**        AA accessibility standards to accommodate
                              users with visual and motor impairments.

  UR-03    **Mobile           The user interface shall provide a fully
           Responsiveness**   responsive layout optimized for mobile,
                              tablet, and desktop screens.

  UR-04    **Error Handling** Clear and context-sensitive error messages
                              shall be displayed for all failed actions
                              (e.g., booking conflict, slot unavailable).

  UR-05    **Help &           Contextual tooltips and brief help popups
           Tooltips**         shall be available on all input fields and
                              actions.

  UR-06    **User             A first-time user tutorial or walkthrough
           Onboarding**       shall be available to guide students in using
                              major features of the portal.
  --------------------------------------------------------------------------

  : []{#_Toc199101195 .anchor}Table 4.18 - Usability Requirements

## Security Requirements

- The system shall enforce secure communication via HTTPS over TLS 1.2
  or higher for all client-server data exchange.

- The system shall encrypt sensitive details like health, counselling,
  and fitness records at rest using AES-256 encryption. This will block
  access to these details from unauthorized users.

- The system shall implement Role-Based Access Control (RBAC) model to
  decide who can view or edit information. Roles such
  as Student and Administrator will manage access to private areas such
  as medical or counselling data.

- The system shall use One-Time Authentication (OTA) for protect
  privileged user accounts and sensitive health or fitness data systems.
  The system delivers One-Time Passwords (OTPs) through email or SMS.
  These passwords stay valid only for a brief period to lower security
  risks.

- Session management plans will include:

<!-- -->

- Automatic logout after inactivity such as 15 minutes.

- Secure handling of authentication tokens.

- Following key practices to avoid Cross-Site Request Forgery
  (CSRF) and Cross-Site Scripting (XSS).

<!-- -->

- The system shall comply with Malaysia Personal Data Protection Act
  (PDPA) and relevant international standards such as GDPR.

## Logical Database Requirements

> The Campus Wellness Portal shall utilize a secure, relational database
> management system (PostgreSQL) to store, retrieve, and manage
> structured wellness data. The schema shall support transactional
> integrity, data security, and efficient query execution for both
> synchronous and asynchronous operations.

### Entities

- **User**: Stores user profiles, credentials (SSO-linked), and role
  assignments.

- **Appointment**: Tracks medical and counselling session bookings with
  associated time, type, provider, and status.

- **CounsellingSession**: Contains confidential session notes,
  participant ID, and assigned counsellor.

- **FitnessClass**: Includes session time, capacity, gender-tag, and
  real-time availability.

- **Goal**: Represents personalized health and wellness goals (e.g.,
  hydration, steps, sleep hours).

- **Notification**: Logs sent messages (email/SMS) for reminders,
  confirmations, and alerts.

- **Feedback**: Captures post-session satisfaction ratings and free-text
  comments.

- **AI_Tip**: Stores generated health insights for user dashboards based
  on tracked metrics.

### Relationships

- **One-to-Many**:

  - User → Appointment, Notification, Feedback

- **Many-to-Many**:

  - User ↔ FitnessClass (via a linking table FitnessBooking)

- **Optional One-to-One**:

  - Appointment → CounsellingSession (if appointment is
    counselling-related)

### Data Integrity Constraints

- All primary keys shall be UUID-based for consistency and security.

- All foreign key references must enforce referential integrity.

- Timestamps (created_at, updated_at) shall be auto-recorded on all
  critical actions (e.g., booking, cancellation).

- Soft delete flags (e.g., is_active, deleted_at) shall be used instead
  of permanent deletions for auditability.

### Security and Access Constraints

- Sensitive fields (e.g., counselling notes) shall be encrypted at rest
  using AES-256.

- Role-Based Access Control (RBAC) policies shall govern field-level
  access, ensuring that only authorized roles (Counsellor, Admin) can
  access protected data.

- Access logs must be maintained to audit database interactions
  involving sensitive data.

### Performance and Optimization

- Indexed fields shall include user_id, appointment_time, status,
  and fitness_class_id.

- Normalized schema shall be applied where feasible to reduce
  redundancy.

- Materialized views or optimized queries may be employed for
  performance-critical features (e.g., live gym slot availability).

# Verification

## Verification Approach

To ensure that all system requirements are correctly and measurably
satisfied, the following multi-layered verification strategy will be
used:

- **How**: Verification will be conducted through a combination of:

  - **Functional Testing** -- to confirm correct behaviour for each use
    case

  - **Unit Testing** -- to validate individual components or functions
    (e.g., login logic, notification handler)

  - **Integration Testing** -- to ensure smooth interaction between
    modules (e.g., login + role routing to admin or student dashboard)

  - **System Testing** -- for end-to-end validation of feature
    workflows(e.g., booking and cancelling appointments)

  - **User Acceptance Testing (UAT)** -- conducted with real student
    users to validate usability and satisfaction.

- **Who:**

  - The Product Team (project developers and analysts) will be
    responsible for conducting functional, unit, and integration
    testing.

  - The Quality Assurance (QA) Team or Advisors will lead UAT and
    document validation results.

- **When:**

  - After each major sprint or milestone (e.g., Sprint 1: Medical
    Services, Sprint 2: Fitness, Sprint 3: Notifications and Reporting).

- **Where:**

  - All tests will be conducted in a controlled staging environment
    simulating MMU's infrastructure and access control protocols.

## Verification Criteria

Each of the following use cases will have specific success criteria for
verification:

+-----------+--------------------+---------------------------------------------------------------------------+
| **Use     | **Use Case Title** | **Verification Criteria**                                                 |
| Case ID** |                    |                                                                           |
+:==========+:===================+:==========================================================================+
| UC01      | Login              | User credentials must be authenticated via SSO, and redirect must occur   |
|           |                    | within 3 seconds.                                                         |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC02      | View Available     | Accurate slot data must be retrieved from database with correct           |
|           | Medical Slots      | doctor/session mapping.                                                   |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC03      | Book Medical       | Slot must be updated in database; confirmation displayed to user          |
|           | Counselling        | immediately.                                                              |
|           | Appointment        |                                                                           |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC04      | Cancel Appointment | Record must be updated; cancelled slot reappears in availability.         |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC05      | Reschedule         | Old appointment is removed, new one added; double-booking is not allowed. |
|           | Appointment        |                                                                           |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC06      | View Counselling   | History is retrieved securely and accurately per student ID.              |
|           | History            |                                                                           |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC07      | View Gym Available | Gym session data must be displayed with date, time, and quota info.       |
|           | Sessions           |                                                                           |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC08      | Book Fitness       | Session booking must update availability count correctly.                 |
|           | Session            |                                                                           |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC09      | Track Wellness     | Metrics shown must match backend calculations (e.g., weight goals, sleep  |
|           | Progress           | logs).                                                                    |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC10      | Set Wellness Goals |   ----------------------------------------------------------------------- |
|           |                    |                                                                           |
|           |                    |   ----------------------------------------------------------------------- |
|           |                    |                                                                           |
|           |                    |   ----------------------------------------------------------------------- |
|           |                    |   Goal inputs must be stored and retrieved correctly.                     |
|           |                    |   ----------------------------------------------------------------------- |
|           |                    |                                                                           |
|           |                    |   ----------------------------------------------------------------------- |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC11      | Get AI Wellness    | AI-generated tip is displayed within 2 seconds and is relevant to user    |
|           | Tips               | profile.                                                                  |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC12      | Receive            | Notification appears within 3 seconds of trigger condition (e.g., 24h     |
|           | Notification       | before session).                                                          |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC13      | Manage             | User preferences are saved and respected in subsequent notifications.     |
|           | Notification       |                                                                           |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC14      | View Student       | Data must aggregate accurately across goals, sessions, and counselling    |
|           | Wellness Report    | logs.                                                                     |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC15      | Manage Fitness     | Admin can create, update, and delete sessions with real-time effect on    |
|           | Class              | student view.                                                             |
+-----------+--------------------+---------------------------------------------------------------------------+
| UC16      | Manage Medical     | Admin can add/edit slots and the frontend reflects changes within 5       |
|           | Schedule           | seconds.                                                                  |
+-----------+--------------------+---------------------------------------------------------------------------+

: []{#_Toc199101196 .anchor}Table 5.1 - Verification Criteria

## Testing Strategy

The Testing Strategy describes how the Campus Wellness Portal shall be
thoroughly tested to ensure that it meets all documented functional and
non-functional requirements. Testing shall be performed on a structured,
iterative basis in accordance with the Agile development lifecycle, with
each sprint providing testable features and components.

### Test Levels and Scope

1.  **Unit Testing**

- Each module (e.g., login form, appointment handler, tip generator)
  will be independently tested by developers.

- Focuses on correctness of logic, input validation, and error handling.

- Automated tools (e.g., PyTest, JUnit) may be used depending on
  implementation.

2.  **Integration Testing**

- Ensures that system modules interact correctly (e.g., login module 🡪
  user role 🡪 appointment dashboard).

- Will include test cases for interactions between frontend forms,
  backend logic, and databases/APIs (e.g., MMU SSO, fitness session
  database).

3.  **System Testing**

- Verifies complete workflows (e.g., Login 🡪 Book Appointment 🡪 View
  History).

- Ensures the system meets its full set of requirements under simulated
  productions conditions.

4.  **User Acceptance Testing (UAT)**

- Real student users will perform end-to-end tasks to evaluate
  usability, correctness, and satisfaction.

- UAT feedback will be used to validate features categorized under
  "Performance" and "Attractive" in the Kano Model.

### Test Artifacts and Deliverables

- **Test Plan**: Defines the testing schedule, responsibilities, tools,
  and resources.

- **Test Cases and Scenarios**: For each use case, specifying:

  - Input Data

  - Expected Output

  - Preconditions and Postconditions

  - Pass/Fail Conditions

- **Test Scripts**: For automation (if applicable) to reduce manual
  testing effort in regression cycles.

- **Defect Log**: Documenting all detected issues, including severity,
  resolution, and test status.

- **Test Summary Report**: Compiles test results, defect trends, and
  final readiness status.

- **UAT Feedback Forms**: Surveys and interview summaries from student
  testers.

### Test Environment

- **QA Testing Environment**: Mirrors the production configuration (web,
  mobile, SSO connectivity, student database) with anonymized test data.

- **Tools**: Testing may use Microsoft Excel/Forms for manual test
  tracking, and automated tools where available.

- **Devices**: System will be tested on Chrome, Firefox, Edge, and
  Android/iOS browsers.

### Test Entry and Exit Criteria

  -----------------------------------------------------------------------
  **Entry Criteria**                  **Exit Criteria**
  ----------------------------------- -----------------------------------
  All planned features and            All test cases executed with ≥ 90%
  functionally complete               pass rate

  Test environment is properly set up All critical defects resolved or
                                      mitigated

  Unit and integration tests are      UAT feedback collected and
  completed                           incorporated
  -----------------------------------------------------------------------

  : []{#_Toc199101197 .anchor}Table 5.2 - Test Entry And Exit Criteria

# Appendices

## Assumptions and Dependencies 

> This section outlines the foundational assumptions made during the
> requirements definition process and identifies critical external
> dependencies that the successful development and operation of the
> Campus Wellness Portal depends upon.

### Assumptions

- **Assumption of User Access:** It is assumed that all end users,
  including students and administrative staff, possess current and
  legitimate MMU Single Sign-On (SSO) credentials, which act as their
  system access authentication method.

- **Device and Network Availability:** It is expected that users have
  access to personal computers (such as laptops, tablets, or
  smartphones) that enable secure HTTPS communication protocols and have
  reliable internet connectivity.

- **User Competence Assumption:** Users are assumed to possess basic
  digital literacy skills necessary to interact with university portals,
  fill forms, manage profiles, and receive notifications through
  standard interfaces.

- **Service Availability of External Systems:** It is assumed that
  university-managed systems---including the MMU Online Portal (for
  authentication), Health System (for medical records), and the Fitness
  Centre Schedule System (for gym session data)---will remain
  operational and accessible during the portal's runtime.

- **Database Stability Assumption:** It is assumed that the Campus
  Wellness Portal's PostgreSQL database will be continuously available,
  with regular backups, transaction logs, and integrity validation
  mechanisms in place to prevent data loss or corruption. Downtime in
  the database layer may affect core operations such as booking, goal
  tracking, and notifications.

### Dependencies

- **System Integration APIs:**

> The portal\'s functionality depends on real-time API availability from
> the []{dir="rtl"}health system, []{dir="rtl"}fitness sessions
> schedule, the university scheduling platform, and notification gateway
> services (e.g., email and SMS dispatch systems).

- **Institutional Data Feeds:**

> The system relies on regular data synchronization with MMU\'s student
> information system (CLiC) for user metadata such as program
> enrollment, faculty assignment, and role designation.

- **Regulatory Compliance:**

> Compliance with MMU IT governance, Malaysian Personal Data Protection
> Act (PDPA), and other relevant privacy regulations is required to
> deploy features involving personal health information (PHI).

- **Middleware Components:**

> For legacy systems lacking modern RESTful interfaces (e.g., older
> modules of CLiC), the portal depends on intermediate middleware or API
> wrappers to bridge communication.

- **Future Expansion Modules:**

> The design assumes future enhancement via AI-based modules (e.g.,
> health coaching, smart goal suggestions) which will require access to
> anonymized historical usage data and behavioural metrics.

## Glossary

> This glossary provides the definitions for key terms that appear in
> the SRS. These will help clarify technical or domain-specific
> vocabulary used throughout the document.

  -------------------------------------------------------------------------
  **Term**         **Definitions**
  ---------------- --------------------------------------------------------
  **Appointment    Backend system module responsible for scheduling,
  Service**        booking, cancelling, and managing medical and
                   counselling appointments.

  **Wellness       A measurable target set by students related to their
  Goal**           health (e.g., number of gym sessions/week).

  **Notification   A system component that generates and dispatches
  Service**        reminders, confirmations, and alerts via email or SMS.

  **Fitness        A structured, scheduled activity (e.g., cardio, yoga)
  Session**        available at the campus gym, bookable via the portal.

  **Single Sign-On Authentication mechanism allowing users to log in once
  (SSO)**          and gain access to multiple systems.

  **OAuth 2.0**    An open protocol for secure delegated access, used for
                   MMU SSO authentication.

  **Counselling    A personal log of previous mental health support
  History**        sessions attended by a student.

  **AI Wellness    Data-driven recommendations generated by an AI module
  Tips**           based on user behavior, goals, or trends.

  **WellnessDB**   Central database that stores user goals, health metrics,
                   and progress tracking information.

  **SMART Goals**  Structured goal-setting framework ensuring goals are
                   Specific, Measurable, Achievable, Relevant, and
                   Time-bound.

  **Student        A compiled overview of a student's activity and
  Wellness         participation in wellness programs.
  Report**         

  **Appointment    A time window available for booking medical counselling
  Slot**           services.

  **Notification   Settings defined by the user for receiving alerts and
  Preferences**    reminders.
  -------------------------------------------------------------------------

  : []{#_Toc199101198 .anchor}Table 6.1 - Glossary

## Acronyms and Abbreviations

  -------------------------------------------------------------------------
  **Acronym**   **Full Term**
  ------------- -----------------------------------------------------------
  **SSO**       Single Sign-On

  **AI**        Artificial Intelligence

  **UAT**       User Acceptance Testing

  **MVP**       Minimum Viable Product

  **DB**        Database

  **MMU**       Multimedia University

  **UC**        Use Case

  **SRS**       Software Requirements Specification

  **UI/UX**     User Interface / User Experience

  **API**       Application Programming Interface

  **DBMS**      Database Management System

  **HTTPS**     Hypertext Transfer Protocol Secure

  **TLS**       Transport Layer Security

  **OTP**       One-Time Password

  **OTA**       One-Time Authentication

  **PDPA**      Personal Data Protection Act (Malaysia)

  **MVP**       Minimum Viable Product

  **RBAC**      Role-Based Access Control

  **CD**        Class Diagram

  **RTM**       Requirements Traceability Matrix

  **KPI**       Key Performance Indicator

  **API**       Application Programming Interface
  -------------------------------------------------------------------------

  : []{#_Toc199101199 .anchor}Table 6.2 - Acronyms and Abbreviations

## User Stories

> User stories offer a simple but powerful way to understand what users
> expect from the system. Instead of focusing on technical details, they
> highlight real needs from the users' point of view. Including these
> stories helps ensure that the system design remains focused on
> providing meaningful value to the people who will use it every day.
> They also support decision-making during development by showing what
> matters most to different user groups.
>
> **Example User Stories**

- I'm a student, and I want to see up-to-the-minute info on gym
  sessions---like, when they're happening, how full they are, and if
  they're men-only, women-only, or whatever---so I can plan my workouts
  without wasting time.

- As a student, I need to book medical appointments online (not by
  calling some dusty office), get a quick confirmation, and reminders so
  I don't forget---basically, I want healthcare on campus to be as
  painless as possible.

- If I'm part of the staff, I want to tweak fitness class schedules on
  the fly---add new classes, shift times, bump up class sizes---so
  students always see what's really available, not last month's
  leftovers.

- And if I'm an admin, I need to pull up detailed reports on who's using
  which wellness programs, sliced by date, activity, or
  demographics---so I can prove the program's worth (or see what's
  flopping) and steer things in the right direction.

> These user stories provide contextual insight into key system features
> described in the Functional Requirements section and serve as a
> reference point for validation during design, development, and user
> acceptance testing.

## Class Diagram 

> **SRS Artifact**\
> **Diagram ID:** CD-01\
> **Version:** 1.0\
> **Date:** 2025-05-23\
> **Author:**  Mohammed Aamena Mohammed Abdulkarem, Mohammed Yousef
> Mohammed Abdulkarem, Nur Thayiebah Binti Hamdan, Farah Hanim Binti
> Mohd Zamri

![Figure 6.1 -- uml Class diagram for campus wellness
portal](media/image36.png){width="7.421386701662292in"
height="5.781052055993001in"}

[]{#_Toc199101148 .anchor}Figure 6.1- UML Class Diagram For Campus
Wellness Portal

### Purpose and Scope

The class diagram in *Figure 6.1* models the core domain entities and
their static relationships within the Campus Wellness Portal system. It
defines the system's static structure by illustrating key classes, their
attributes, operations, and the associations, generalizations, and
dependencies among them. This diagram and its description serve as
foundational artifacts to support requirements specification, and to
guide system design, implementation, and verification activities.

### Classes and Responsibilities

- **User (Abstract Class)**

> Represents a generic system user with common attributes such
> as userID: String, name: String, email: String, and authentication
> credentials (passwordHash: String). This abstract class provides a
> common interface and behavior for all user types, promoting reuse and
> consistent user management across the system.

- **Student (Subclass of User)**

> Models the primary actor interacting with wellness services. Students
> can view and book appointments, set wellness goals, track progress,
> and access fitness sessions. Attributes include studentID:
> String, preferences: PreferencesType, and profileStatus: Enum.
> Operations include booking management and goal tracking.

- **Admin (Subclass of User)**

> Represents administrative staff responsible for managing schedules,
> monitoring system usage, and maintaining data integrity. Admins have
> elevated privileges for system configuration, user management, and
> oversight.

- **Appointment**

> Encapsulates booking details for medical or counseling sessions, with
> attributes such as appointmentID: String, dateTime: DateTime, status:
> Enum {Scheduled, Cancelled, Completed}, and associatedUser: User.
> Operations include creation, modification, cancellation, and
> notification triggering.

- **FitnessSession**

> Defines gym or fitness class sessions with attributes like sessionID:
> String, startTime: DateTime, capacity: Integer, genderRestriction:
> Enum {Male, Female, None}, and currentEnrollment: Integer. Supports
> availability checking and booking management.

- **WellnessGoal**

> Represents personal wellness objectives set by students, characterized
> by goalID: String, activityType: String, frequencyPerWeek:
> Integer, durationInWeeks: Integer, and progress: Float. Supports
> validation according to SMART goal principles and triggers
> notification events upon progress milestones.

- **Notification**

> Manages communication with users, including booking confirmations,
> cancellations, reminders, and motivational messages. Attributes
> include notificationID: String, type: Enum, deliveryStatus: Enum,
> and timestamp: DateTime. Integrates with external email and SMS
> services ensuring reliable and timely delivery with retry mechanisms.

### Relationships

- **Generalization (Inheritance)**

> The abstract **User** class is specialized
> into **Student** and **Admin** classes. This generalization
> is *complete* and *disjoint*, ensuring every User instance is either a
> Student or an Admin, but never both. This constraint is explicitly
> modeled in UML with the {complete, disjoint} notation.

- **Associations**

  - **Student** is associated with
    multiple **Appointment**, **FitnessSession**,
    and **WellnessGoal** instances, representing the student's
    interactions with wellness services.

  - **Appointment** is linked to a single **User** (either Student or
    Admin), indicating booking ownership and administrative oversight.

  - **Notification** is associated with **User**, representing
    communication channels to individual users.

- **Multiplicity and Navigability**

  - A **Student** may have zero or many (0..\*) **Appointments**.

  - An **Appointment** is linked to exactly one (1) **User**.

  - A **FitnessSession** can have multiple enrolled Students up to its
    capacity.

  - Navigability arrows indicate that the system can retrieve a
    Student's appointments and send Notifications to Users.

### Constraints and Business Rules

- **Role Exclusivity:**

> A User instance must be exclusively either a Student or an Admin,
> never both, enforcing security and operational policies.

- **Appointment Integrity:**

> Appointments must be linked to authenticated Students and managed or
> approved by Admins to ensure valid scheduling, avoid conflicts, and
> maintain data consistency.

- **Session Capacity:**

> FitnessSession enforces capacity limits and gender-specific
> restrictions to comply with wellness center policies. Overbooking is
> prevented.

- **Goal Validation:**

> WellnessGoal entries must comply with predefined formats and ranges
> (e.g., frequency per week must be a positive integer within allowed
> limits), supporting SMART goal criteria.

- **Notification Reliability:**

> Notifications must be delivered reliably and timely, with automated
> retry attempts for delivery failures and confirmation of receipt
> logged.

### Traceability to Requirements

> Each class and relationship supports specific functional and
> non-functional requirements documented in the system requirements
> specification (SRS):

- The **Student** and **Appointment** classes directly fulfill use cases
  related to booking, rescheduling, and cancelling appointments.

- The **FitnessSession** class supports use cases for viewing and
  booking fitness classes with real-time availability.

- The **WellnessGoal** and **Notification** classes enable personal goal
  setting, progress tracking, and motivational feedback, supporting user
  engagement.

> These mappings ensure traceability from system requirements through to
> design artifacts, facilitating verification, validation, and impact
> analysis.

### Compliance with ISO/IEC/IEEE 29148:2018

> This class diagram description follows ISO/IEC/IEEE 29148:2018
> guidelines for clarity, precision, and traceability, ensuring the
> artifact supports verifiable and consistent system design aligned with
> stakeholder requirements.

## Requirement Traceability Matrix (RTM)

  -----------------------------------------------------------------------------------
  **Requirement   **Description**   **Use Case     **Source**       **Verification
  ID**                              ID**                            Method**
  --------------- ----------------- -------------- ---------------- -----------------
  REQ-01          Secure SSO Login  UC-01          Questionnaire    System Test
                                                                    (Valid/Invalid
                                                                    Login Flow)

  REQ-02          Real-time Medical UC-02          Questionnaire,   System Test (Slot
                  Slot Viewing                     Observation      Retrieval)

  REQ-03          Book Medical      UC-03          Questionnaire,   Integration Test
                  Appointment                      Observation      (Booking and
                                                                    Database)

  REQ-04          Cancel            UC-04          Questionnaire    System Test
                  Appointment                                       (Cancel +
                                                                    Feedback Message)

  REQ-05          Reschedule        UC-05          Questionnaire    System Test
                  Appointment                                       (Rescheduling
                                                                    Workflow)

  REQ-06          View Counselling  UC-06          Questionnaire    System Test
                  History                                           (Authenticated
                                                                    Data Access)

  REQ-07          View Fitness      UC-07          Questionnaire    System Test
                  Sessions (Incl.                                   (Session Listing
                  Gender-Specific                                   Logic)
                  Options)                                          

  REQ-08          Book Fitness      UC-08          Questionnaire    Integration Test
                  Session                                           (Booking Module
                                                                    and Database)

  REQ-09          Track Wellness    UC-09          Questionnaire    System Test
                  Progress                                          (Chart Display
                                                                    Logic)

  REQ-10          Set Wellness      UC-10          Questionnaire    System Test (Goal
                  Goals                                             Saving + Update)

  REQ-11          AI Wellness Tips  UC-11          Brainstorming,   Simulation/Unit
                                                   Questionnaire    Testing (AI Tip
                                                                    Generation)

  REQ-12          Receive           UC-12          Questionnaire    System Test
                  Notifications                                     (Trigger and
                                                                    Delivery)

  REQ-13          Manage            UC-13          Brainstorming,   System Test
                  Notification                     Observation      (Preferences
                  Preferences                                       Saved Correctly)

  REQ-14          View Wellness     UC-14          Brainstorming,   System Test
                  Report                           Observation      (Report
                                                                    Generation and
                                                                    Viewing)

  REQ-15          Manage Fitness    UC-15          Observation      Integration Test
                  Class                                             (Admin UI +DB
                                                                    Update)

  REQ-16          Manage Medical    UC-16          Observation      Integration Test
                  Schedule                                          (Class
                                                                    Scheduling +
                                                                    Admin Interface)
  -----------------------------------------------------------------------------------

  : []{#_Toc199101200 .anchor}Table 6.3 - Requirement Traceability
  Matrix

## Supporting Materials

### Kano Model Questionnaire Results

<figure>
<img src="media/image37.png" style="width:6.26806in;height:1.30303in"
alt="A screenshot of a computer AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101149" class="anchor"></span>Figure 6.2
- Questionnaire Board</p></figcaption>
</figure>

Responses were collected using the questionnaire shown in *Figure 6.2:
Questionnaire Board.*

<figure>
<img src="media/image37.png" style="width:6.26806in;height:2.07576in"
alt="A screenshot of a computer AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101150" class="anchor"></span>Figure 6.3
- Questionnaire Results (User Satisfaction With SSO)</p></figcaption>
</figure>

**Figure 6.3:** The system shall provide a secure Single Sign-On (SSO)
mechanism for users to log in to the Campus Wellness Portal with a
single click. Out of 20 respondents, 16 (80%) \"like it,\" 2 (10%)
\"expect it,\" 1 (5%) is \"neutral,\" and 1 (5%) \"can tolerate it.\" No
respondents \"dislike it.\"

<figure>
<img src="media/image37.png" style="width:6.26806in;height:2.07443in"
alt="A screenshot of a computer AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101151" class="anchor"></span>Figure 6.4
- Questionnaire Results (User Satisfaction With Slots
Viewing)</p></figcaption>
</figure>

**Figure 6.4:** The system shall enable users to view all available
medical appointment slots in real-time on the Campus Wellness Portal.
Out of 20 respondents, 12 (60%) \"like it,\" 7 (35%) \"expect it,\" and
1 (5%) is \"neutral.\" No respondents \"can tolerate it\" or \"dislike
it.\"

<figure>
<img src="media/image38.png" style="width:6.26806in;height:1.90385in"
alt="A screenshot of a computer AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101152" class="anchor"></span>Figure 6.5
- Questionnaire Results (User Satisfaction With Appointment
Booking)</p></figcaption>
</figure>

**Figure 6.5:** The system shall facilitate the easy booking of medical
counselling appointments through the Campus Wellness Portal. Out of 20
respondents, 17 (85%) \"like it\" and 3 (15%) \"expect it.\" No
respondents are \"neutral,\" \"can tolerate it,\" or \"dislike it.\"

<figure>
<img src="media/image38.png" style="width:6.26712in;height:2.00641in"
alt="A screenshot of a computer AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101153" class="anchor"></span>Figure 6.6
- Questionnaire Results (User Satisfaction With Cancel/Reschedule
Appointment)</p></figcaption>
</figure>

**Figure 6.6:** The system shall allow users to easily cancel or
reschedule their medical appointments through the Campus Wellness
Portal. Out of 20 respondents, 14 (70%) \"like it,\" 4 (20%) \"expect
it,\" and 2 (10%) are \"neutral.\" No respondents \"can tolerate it\" or
\"dislike it.\"

<figure>
<img src="media/image38.png" style="width:6.26806in;height:1.9563in"
alt="A screenshot of a computer AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101154" class="anchor"></span>Figure 6.7
- Questionnaire Results (User Satisfaction With History
Viewing)</p></figcaption>
</figure>

**Figure 6.7:** The system shall provide users with the ability to view
their complete counselling history directly on the Campus Wellness
Portal. Out of 20 respondents, 14 (70%) \"like it,\" 4 (20%) \"expect
it,\" and 2 (10%) are \"neutral.\" No respondents \"can tolerate it\" or
\"dislike it.\"

<figure>
<img src="media/image39.png" style="width:6.26806in;height:1.85256in"
alt="A screenshot of a cell phone AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101155" class="anchor"></span>Figure 6.8
- Questionnaire Results (User Satisfaction With Tracking Wellness
Progress)</p></figcaption>
</figure>

**Figure 6.8:** The system shall enable users to track their wellness
progress (e.g., activity levels, health metrics) through the Campus
Wellness Portal. Out of 20 respondents, 15 (75%) \"like it,\" 3 (15%)
\"expect it,\" and 2 (10%) are \"neutral.\" No respondents \"can
tolerate it\" or \"dislike it.\"

<figure>
<img src="media/image39.png" style="width:6.26744in;height:2.00604in"
alt="A screenshot of a cell phone AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101156" class="anchor"></span>Figure 6.9
- Questionnaire Results (User Satisfaction With Setting Personal
Goals)</p></figcaption>
</figure>

**Figure 6.9:** The system shall allow users to set personalized
wellness goals (e.g., daily steps, water intake) on the Campus Wellness
Portal. Out of 20 respondents, 13 (65%) \"like it,\" 3 (15%) \"expect
it,\" and 4 (20%) are \"neutral.\" No respondents \"can tolerate it\" or
\"dislike it.\"

<figure>
<img src="media/image39.png" style="width:6.26667in;height:1.86471in"
alt="A screenshot of a cell phone AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101157" class="anchor"></span>Figure
6.10 - Questionnaire Results (User Satisfaction With Provided
Tips)</p></figcaption>
</figure>

**Figure 6.10:** The system shall provide users with personalized
wellness tips through the Campus Wellness Portal. Out of 20 respondents,
11 (55%) \"like it,\" 2 (10%) \"expect it,\" 5 (25%) are \"neutral,\"
and 2 (10%) \"can tolerate it.\" No respondents \"dislike it.\"

<figure>
<img src="media/image40.png" style="width:6.26599in;height:1.86538in"
alt="A screenshot of a test AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101158" class="anchor"></span>Figure
6.11 - Questionnaire Results (User Satisfaction With Sessions
Viewing)</p></figcaption>
</figure>

**Figure 6.11:** The system shall enable users to view available fitness
class sessions in real-time on the Campus Wellness Portal. Out of 20
respondents, 14 (70%) \"like it,\" 3 (15%) \"expect it,\" and 3 (15%)
are \"neutral.\" No respondents \"can tolerate it\" or \"dislike it.\"

<figure>
<img src="media/image40.png" style="width:6.26512in;height:2.00609in"
alt="A screenshot of a test AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101159" class="anchor"></span>Figure
6.12 - Questionnaire Results (User Satisfaction With Sessions
Booking)</p></figcaption>
</figure>

**Figure 6.12:** The system shall facilitate the easy booking of fitness
sessions through the Campus Wellness Portal. Out of 20 respondents, 14
(70%) \"like it,\" 4 (20%) \"expect it,\" and 2 (10%) are \"neutral.\"
No respondents \"can tolerate it\" or \"dislike it.\"

<figure>
<img src="media/image40.png" style="width:6.26528in;height:1.84583in"
alt="A screenshot of a test AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101160" class="anchor"></span>Figure
6.13 - Questionnaire Results (User Satisfaction With Notification And
Reminders)</p></figcaption>
</figure>

**Figure 6.13:** The system shall provide notifications and reminders to
users for upcoming appointments and fitness classes via the Campus
Wellness Portal. Out of 20 respondents, 14 (70%) \"like it,\" 4 (20%)
\"expect it,\" 1 (5%) is \"neutral,\" 1 (5%) \"can tolerate it,\" and 0
(0%) \"dislike it.\"

<figure>
<img src="media/image41.png" style="width:6.2674in;height:1.82051in"
alt="A screenshot of a graph AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101161" class="anchor"></span>Figure
6.14 - Questionnaire Results (User Satisfaction With Gender-Specific
Sessions Viewing)</p></figcaption>
</figure>

**Figure 6.14:** The system shall enable users to view and book
gender-specific gym sessions to accommodate cultural preferences on the
Campus Wellness Portal. Out of 20 respondents, 17 (85%) \"like it,\" 3
(15%) \"expect it,\" and 0 (0%) were neutral, could tolerate, or
disliked it.

<figure>
<img src="media/image41.png" style="width:6.26797in;height:1.82051in"
alt="A screenshot of a graph AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101162" class="anchor"></span>Figure
6.15 - Questionnaire Results (Dysfunction of SSO)</p></figcaption>
</figure>

**Figure 6.15:** The system shall ensure secure login functionality for
the Campus Wellness Portal. User feedback strongly indicates a negative
sentiment towards the absence of secure login, with 16 out of 20
respondents (80%) \"disliking it,\" 2 (10%) \"liking it\" (likely
misinterpreted), 1 (5%) \"expecting it\" (likely misinterpreted), and 1
(5%) able to \"tolerate it.\"

<figure>
<img src="media/image41.png" style="width:6.26623in;height:2.01282in"
alt="A screenshot of a graph AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101163" class="anchor"></span>Figure
6.16 - Questionnaire Results (Dysfunction of Slots
Viewing)</p></figcaption>
</figure>

**Figure 6.16:** The system shall provide users with the ability to view
available medical slots in real-time on the Campus Wellness Portal. User
feedback reveals a strong negative sentiment towards the inability to
view real-time slots, with 11 out of 20 respondents (55%) \"disliking
it\" and 7 (35%) able to \"tolerate it.\" 2 respondents (10%) \"like
it\" (likely misinterpreted), and 0 \"expect it\" or are \"neutral.\"

<figure>
<img src="media/image42.png" style="width:6.26806in;height:1.78846in"
alt="A screenshot of a computer screen AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101164" class="anchor"></span>Figure
6.17 - Questionnaire Results (Dysfunction of Appointment
Booking)</p></figcaption>
</figure>

**Figure 6.17:** The system shall enable users to book medical
counselling appointments through the Campus Wellness Portal. User
feedback indicates a significant negative reaction to the inability to
book appointments, with 12 out of 20 respondents (60%) \"disliking it\"
and 6 (30%) able to \"tolerate it.\" 2 respondents (10%) \"like it\"
(likely misinterpreted), and 0 \"expect it\" or are \"neutral.\"

<figure>
<img src="media/image42.png" style="width:6.26731in;height:1.96154in"
alt="A screenshot of a computer screen AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101165" class="anchor"></span>Figure
6.18 - Questionnaire Results (Dysfunction of Cancel/Rescheduling
Appointments)</p></figcaption>
</figure>

**Figure 6.18:** The system shall allow users to cancel or reschedule
medical appointments through the Campus Wellness Portal. Out of 20
respondents, 13 (65%) \"dislike it\" if unable to do so, 4 (20%) \"can
tolerate it,\" 1 (5%) is \"neutral,\" 1 (5%) \"expect it,\" and 1 (5%)
\"like it.\"

<figure>
<img src="media/image42.png" style="width:6.26756in;height:2.01725in"
alt="A screenshot of a computer screen AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101166" class="anchor"></span>Figure
6.19 - Questionnaire Results (Dysfunction of History
Viewing)</p></figcaption>
</figure>

**Figure 6.19:** The system shall enable users to view their counselling
history securely on the Campus Wellness Portal. Out of 20 respondents, 8
(40%) \"dislike it\" if unable to view, 7 (35%) \"can tolerate it,\" 3
(15%) are \"neutral,\" and 2 (10%) \"like it.\"

<figure>
<img src="media/image43.png" style="width:6.26806in;height:1.90385in"
alt="A screenshot of a survey AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101167" class="anchor"></span>Figure
6.20 - Questionnaire Results (Dysfunction of Tracking Wellness
Progress)</p></figcaption>
</figure>

**Figure 6.20:** The system shall enable users to track their wellness
progress on the Campus Wellness Portal. Out of 20 respondents, 9 (45%)
\"dislike it\" if unable to track progress, 6 (30%) \"can tolerate it,\"
3 (15%) are \"neutral,\" 2 (10%) \"like it,\" and 0 (0%) \"expect it.\"

<figure>
<img src="media/image43.png" style="width:6.26728in;height:2in"
alt="A screenshot of a survey AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101168" class="anchor"></span>Figure
6.21 - Questionnaire Results (Dysfunction of Setting Personal
Goals)</p></figcaption>
</figure>

**Figure 6.21:** The system shall enable users to set personalized
wellness goals on the Campus Wellness Portal. Out of 20 respondents, 9
(45%) \"dislike it\" if unable to set goals, 7 (35%) \"can tolerate
it,\" 2 (10%) are \"neutral,\" 2 (10%) \"like it,\" and 0 (0%) \"expect
it.\"

<figure>
<img src="media/image43.png" style="width:6.26664in;height:1.80128in"
alt="A screenshot of a survey AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101169" class="anchor"></span>Figure
6.22 - Questionnaire Results (Dysfunction of Providing
Tips)</p></figcaption>
</figure>

**Figure 6.22:** The system shall provide wellness tips to users through
the Campus Wellness Portal. Out of 20 respondents, 8 (40%) \"dislike
it\" if not receiving tips, 4 (20%) \"can tolerate it,\" 5 (25%) are
\"neutral,\" 2 (10%) \"like it,\" and 1 (5%) \"expect it.\"

<figure>
<img src="media/image44.png" style="width:6.26806in;height:1.92308in"
alt="A screenshot of a test AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101170" class="anchor"></span>Figure
6.23 - Questionnaire Results (Dysfunction of Sessions
Viewing)</p></figcaption>
</figure>

**Figure 6.23:** The system shall enable users to view available fitness
class sessions on the Campus Wellness Portal. Out of 20 respondents, 11
(55%) \"dislike it\" if unable to view classes, 4 (20%) \"can tolerate
it,\" 3 (15%) are \"neutral,\" 2 (10%) \"like it,\" and 0 (0%) \"expect
it.\"

<figure>
<img src="media/image44.png" style="width:6.26797in;height:1.96154in"
alt="A screenshot of a test AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101171" class="anchor"></span>Figure
6.24 - Questionnaire Results (Dysfunction of Sessions
Booking)</p></figcaption>
</figure>

**Figure 6.24:** The system shall enable users to book fitness sessions
through the Campus Wellness Portal. Out of 20 respondents, 8 (40%)
\"dislike it\" if unable to book sessions, 7 (35%) \"can tolerate it,\"
3 (15%) are \"neutral,\" 1 (5%) \"like it,\" and 1 (5%) \"expect it.\"

<figure>
<img src="media/image44.png" style="width:6.26667in;height:1.74903in"
alt="A screenshot of a test AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101172" class="anchor"></span>Figure
6.25 - Questionnaire Results (Dysfunction of Notification and
Reminders)</p></figcaption>
</figure>

**Figure 6.25:** The system shall provide notifications and reminders to
users through the Campus Wellness Portal. Out of 20 respondents, 11
(55%) \"dislike it\" if not receiving notifications, 5 (25%) \"can
tolerate it,\" 2 (10%) are \"neutral,\" 2 (10%) \"like it,\" and 0 (0%)
\"expect it.\"

<figure>
<img src="media/image45.png" style="width:6.26806in;height:1.90385in"
alt="A purple circle with black text AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101173" class="anchor"></span>Figure
6.26 - Questionnaire Results (Dysfunction of Gender-Specific Sessions
Viewing)</p></figcaption>
</figure>

**Figure 6.26:** The system shall enable users to view and book
gender-specific gym sessions through the Campus Wellness Portal. Out of
20 respondents, 12 (60%) \"dislike it\" if unable to view/book
gender-specific sessions, 5 (25%) \"can tolerate it,\" 1 (5%) is
\"neutral,\" 2 (10%) \"like it,\" and 0 (0%) \"expect it.\"

###  Kano Model Analysis 

  --------------------------------------------------------------------------------------
  Features                  Satisfaction   Functionality   \"Consumer Need Level
                                                           (\"\"Expected Need\"\",
                                                           \"\"Normal Need\"\", and
                                                           \"\"Exciting Need\"\")\"
  ------------------------- -------------- --------------- -----------------------------
  Wellness Goals Setting    3              3               Normal Need

  Book Fitness Session      4              4               Normal Need

  Book Medical Appointment  1              5               Expected Need

  Cancel/Reschedule         4              4               Normal Need
  Appointment                                              

  View Counselling History  3              3               Normal Need

  Gender-Specific Gym       3              4               Normal Need
  Sessions                                                 

  Notifications/Reminders   3              4               Normal Need

  Real-time Medical Slots   1              3               Expected Need

  Secure SSO Login          1              4               Expected Need

  Track Wellness Progress   3              3               Normal Need

  View Fitness Sessions     3              5               Normal Need

  AI Wellness Tips          5              1               Exciting Need

  Manage Notification       5              3               Exciting Need

  View Student Wellness     5              2               Exciting Need
  Report                                                   

  Manage Fitness Class      5              4               Normal Need

  Manage Medical Schedule   2              5               Expected Need
  --------------------------------------------------------------------------------------

  : []{#_Toc199101201 .anchor}Table 6.4 - Kano Functional Classification
  with Satisfaction-Functionality with Results

<figure>
<img src="media/image46.png" style="width:6.26528in;height:4.16667in"
alt="A graph of different colored lines AI-generated content may be incorrect." />
<figcaption><p><span id="_Toc199101174" class="anchor"></span>Figure
6.27 - Kano Model Diagram</p></figcaption>
</figure>

**Figure 6.27:** Presents a Kano Analysis chart that maps the functional
requirements of the Campus Wellness Portal based on their impact on user
satisfaction (y-axis) and their level of implementation (x-axis). Each
requirement is plotted according to its classification derived from
structured Kano questionnaire responses, stakeholder brainstorming, and
contextual observations. Features classified as *Must-be*---such
as Secure SSO Login, Book Medical Appointment, and Real-time Medical
Slot Viewing---are positioned along the baseline of user expectations,
where their absence would result in strong
dissatisfaction. *One-Dimensional* features such as Reschedule
Appointment, Track Wellness Progress, and Book Fitness Session exhibit a
linear relationship between performance and satisfaction, indicating
that better implementation directly improves user experience.
Finally, *Attractive* features---such as AI Wellness Tips, Manage
Notification Preferences, and View Wellness Report---occupy the
upper-right quadrant, highlighting their potential to delight users even
though they are not expected by default. This visualization supports
strategic prioritization by clearly distinguishing between essential,
performance-based, and value-adding features within the system.

#### Must-be (Basic) Requirements

> These are essential for baseline functionality:

- **REQ-01:** Secure SSO Login

- **REQ-02:** Real-time Medical Slots

- **REQ-03:** Book Medical Appointment

- **REQ-16:** Manage Medical Schedule

#### One-dimensional (Satisfiers)

> These features provide proportional increases in user satisfaction
> based on the quality of implementation:

- **REQ-04:** Cancel Appointment

- **REQ-05:** Reschedule Appointment

- **REQ-06:** View Counselling History

- **REQ-07:** View Fitness Sessions with Gender-Specific Gym Options

- **REQ-08:** Book Fitness Session

- **REQ-09:** Track Wellness Progress

- **REQ-10:** Set Wellness Goals

- **REQ-12:** Receive Notification

- **REQ-15:** Manage Fitness Class

#### Attractive (Delighters)

> These features exceed baseline expectations and foster user delight:

- **REQ-11:** AI Wellness Tips

- **REQ-13:** Manage Notification

- **REQ-14:** View Student Wellness Report**\**

### Observation Checklist 

> **MMU Online Portal and Campus Wellness Systems**
>
> **Observation Team:**
>
> FARAH HANIM BINTI MOHD ZAMRI
>
> NUR THAYIEBAH BINTI HAMDAN
>
> MOHAMMED AAMENA MOHAMMED ABDULKAREM
>
> MOHAMMED YOUSEF MOHAMMED ABDULKAREM
>
> **Date**: 25 April 2025
>
> **Location**: MMU Center / Online Review
>
> **Observation Method**: In-person / Video-Based Analysis

  -----------------------------------------------------------------------------------
  **Observation Point**                                      **Status**   **Notes**
  ---------------------------------------------------------- ------------ -----------
  User successfully authenticates via MMU Online Portal      ☑            

  User navigates to wellness-related features (e.g.,         ☑            
  appointment booking, scheduling) with minimal support                   

  System errors or delays encountered during interaction     ☑            

  User demonstrates understanding of key functionalities     ☑            

  Use of help/search functionality if difficulties arise     ☑            

  Behavioural signs of confusion or hesitation observed      ☑            

  Preference for real-time availability explicitly noted or  ☑            
  implied                                                                 
  -----------------------------------------------------------------------------------

  : []{#_Toc199101202 .anchor}Table 6.5 - User Interaction and Behaviour
  Checklist

  --------------------------------------------------------------------------------
  **Observation Point**                                   **Status**   **Notes**
  ------------------------------------------------------- ------------ -----------
  User attempts to schedule/reschedule an appointment     ☑            

  Interface design supports intuitive scheduling          ☑            

  Bottlenecks in the appointment workflow identified      ☑            

  Appointment details successfully confirmed by user      ☑            

  User engages with reminder/calendar feature (if         ☑            
  available)                                                           
  --------------------------------------------------------------------------------

  : []{#_Toc199101203 .anchor}Table 6.6 - Scheduling and Appointment
  Management Checklist

  -------------------------------------------------------------------------------
  **Observation Point**                                  **Status**   **Notes**
  ------------------------------------------------------ ------------ -----------
  Portal operations align with standard clinical         ☑            
  workflows                                                           

  Devices and configurations function as per guidelines  ☑            

  No significant workflow disruptions observed           ☑            
  -------------------------------------------------------------------------------

  : []{#_Toc199101204 .anchor}Table 6.7 - Functional Workflow and CLiC
  Compliance Checklist

  --------------------------------------------------------------------------------
  **Observation Point**                                   **Status**   **Notes**
  ------------------------------------------------------- ------------ -----------
  UI layout and navigation are clear and accessible       ☑            

  Text and iconography meet usability and legibility      ☑            
  standards                                                            

  Navigation structure aligns with user expectations      ☑            

  System feedback messages are visible and meaningful     ☑            

  System responsiveness meets performance thresholds      ☑            
  --------------------------------------------------------------------------------

  : []{#_Toc199101205 .anchor}Table 6.8 - User Interface and Experience
  Checklist

  --------------------------------------------------------------------------------
  **Observation Point**                                   **Status**   **Notes**
  ------------------------------------------------------- ------------ -----------
  User actions in videos mirror live observations         ☑            

  Key usability challenges consistently identified        ☑            

  No major deviation between recorded and live behaviour  ☑            
  --------------------------------------------------------------------------------

  : []{#_Toc199101206 .anchor}Table 6.9 - Supplementary Video
  Observations Checklist

**General Notes and Key Findings**

- Fragmented navigation between portals creates usability friction.

- Students appreciated scheduling functions but faced difficulties with
  slot availability interpretation.

- The absence of gamification or interactive wellness tracking features
  was noticeable.

- Interface guidance and onboarding tools were lacking.

- System stability was consistent, with minor performance lag during
  peak access times.

**Summary of Bottlenecks and Recommendations**

  -----------------------------------------------------------------------
  **Identified            **Observed Impact**   **Suggested
  Bottleneck**                                  Recommendation**
  ----------------------- --------------------- -------------------------
  Portal-to-portal        User confusion and    Implement unified
  navigation              inefficiency          navigation framework
  inconsistency                                 

  Lack of real-time       Inefficient booking   Integrate dynamic slot
  availability indicators process               visibility

  Complex appointment     User error and        Simplify interface and
  workflow                abandonment           reduce steps

  Unclear access to       Underutilization of   Enhance
  wellness tools          features              tooltips/tutorials

  Variable system load    Reduced satisfaction  Conduct performance
  times                   during peaks          optimization
  -----------------------------------------------------------------------

  : []{#_Toc199101207 .anchor}Table 6.10 - Summary of Bottlenecks and
  Recommendations

### Meeting Minutes and Brainstorm Notes

Teams Meeting

Sun, May 18, 2025

Summary:

The session focused on brainstorming AI functionalities to enhance the
student experience within the campus wellness portal. Participants
discussed the structure of the session, including the order of
presentations and the necessity for a rehearsal. Farah expressed her
readiness to present first, while Mohammed Aamena proposed a
collaborative discussion format. The team agreed to concentrate on
specific areas of interest and planned to rehearse prior to the actual
presentation.

During the brainstorming, Farah introduced several AI-driven features,
such as secure login enhancements, AI-assisted counseling history
analysis, and personalized notifications for wellness activities. Aamina
contributed ideas on tracking wellness progress and streamlining gym
booking processes, while Taiba emphasized the importance of generating
personalized wellness tips and ensuring data privacy. The group aimed to
compile a refined list of features that directly address student needs,
with a focus on integrating AI effectively into the portal.

The discussion then shifted to prioritizing features for the initial
implementation phase. Farah highlighted the critical need for data
security, particularly concerning health information. There was some
confusion regarding the discussion structure, prompting Nur to seek
clarification. Mohammed Aamena suggested a more interactive approach to
enhance engagement, leading to an acknowledgment of the need for a
dynamic dialogue to address implementation effectively.

The team concluded by agreeing on the importance of tailoring AI fitness
suggestions to student activities and preferences. Farah proposed
strategies for managing incorrect AI suggestions, including user
feedback and customization options. Mohammed Yousef emphasized the
necessity of providing students with control over AI features to foster
trust and privacy. The session wrapped up with plans to prepare a
validation survey for student feedback, ensuring that the proposed
functionalities align with user expectations.

Chapters & Topics:

Focused Brainstorming Session on AI Functionalities for Student Wellness
Portal

Mohammed Yousef Mohammed Abdulkarem led a brainstorming session focused
on defining AI functionalities for the campus wellness portal. The group
discussed the session\'s format, including who would present and in what
order. Farah Hanim Binti Mohd Zamri and Mohammed Aamena Mohammed
Abdulkarem contributed to the planning of the session, emphasizing the
importance of rehearsing before the actual presentation.

AI-Driven Enhancements for Campus Wellness Portal

Mohammed Yousef initiated the discussion on enhancing the campus
wellness portal with AI functionalities aimed at improving student
experiences. Farah highlighted key areas such as secure logins,
AI-driven counseling analysis, and personalized wellness notifications.
Amina focused on wellness tracking, goal setting, and gym booking
suggestions, while Taiba emphasized the importance of personalized
wellness tips, smart notifications, and privacy controls. Each speaker
contributed to a collaborative effort to refine potential AI features.

\* Secure login and authentication enhancements

Collaborative Discussion on Phase One Features

Mohammed Yousef prompted a discussion regarding the features that should
be prioritized for phase one implementation. Farah highlighted the
critical need for data security and privacy, especially concerning
health-related information. The dialogue included some confusion about
the collaborative format, with participants expressing a desire for a
more interactive discussion before moving to a summary.

Collaborative Discussion on AI Features and Implementation

Mohammed Yousef highlighted the necessity of AI-driven booking
suggestions and the integration of AI tips. The team discussed the
terminology for their project, leaning towards calling their ideas
features rather than use cases. Farah suggested structuring their
collaborative discussion around specific agenda items, while the group
prepared questions for each other to facilitate the discussion.

AI-Driven Fitness Recommendations and User Control

Aamina outlined methods to make AI fitness suggestions relevant to
students\' activities, including allowing users to select how often they
receive tips and ensuring messages are concise. Nur added that
recommendations should consider both user preferences and performance
data to enhance personalization. Farah suggested implementing user
feedback mechanisms and automated monitoring to address inappropriate
suggestions, emphasizing the need for transparency and user control over
AI features.

AI-Driven Functionalities for Campus Wellness Portal

Mohammed Yousef initiated a brainstorming session focused on AI
functionalities for the campus wellness portal, emphasizing the
importance of aligning features with student needs. Farah Hanim and
Mohammed Aamina supported the proposed ideas, which included smart
scheduling and adaptive wellness suggestions. The group agreed to create
a validation survey for student feedback as a follow-up action.

\* AI-assisted counseling and wellness tracking

\* AI-driven functionalities for enhancing student experience in
wellness portal

AI-Enhanced Wellness System Features Presentation

Farah outlined key features for the AI-Enhanced Wellness System,
including secure login with multi-factor authentication and AI risk
detection. She highlighted the use of natural language processing for
analyzing counseling histories, personalized notifications for wellness
activities, and automated reporting to track student progress.
Additionally, she proposed smart fitness class management that adjusts
based on demand and user preferences.

\* Personalized notifications and reminders

Enhancing Student Wellness and Goal Setting through AI

Mohammed Aameena Mohammed AbdulKarem outlined strategies to enhance
student wellness through AI. The proposed features include tracking
wellness habits, suggesting realistic goals based on past behavior,
providing daily wellness tips, and recommending gym booking slots
tailored to students\' schedules. These initiatives aim to keep students
engaged and motivated in their wellness journeys.

Enhancing the Campus Wellness Portal with AI

Mohammed Aameena discussed the potential of making the campus wellness
portal more supportive for students, especially during exams and
assignments. Taiba presented suggestions for AI-driven wellness tips
tailored to student habits, improved notification management, and strong
privacy controls. These enhancements aim to create a more personalized
and trustworthy experience for users.

\* Privacy and transparency in AI data usage

Collaborative Discussion on Project Documentation

The team discussed the best approach for managing project documentation,
particularly the SRS, with suggestions to use both GitHub and Word.
Mohammed Aamena emphasized the need for collaboration and sharing files
before pushing them to GitHub, while Farah Hanim expressed concerns
about ensuring proper comments and commits to meet the lecturer\'s
expectations. Mohammed Yousef supported the idea of using GitHub for
tracking contributions.

\* Division of responsibilities for the SRS document.

Discussion on Elicitation Plan and SRS Diagrams

Farah and Mohammed reviewed the elicitation plan, with Farah asking for
it once completed. They confirmed the requirement for at least two
diagrams for each use case and discussed the need to identify a
consistent table format for the use case diagram. They agreed to finish
the initial documents before moving on to the Software Requirements
Specification (SRS).

\* Elicitation plan and its timeline for sharing.

\* Identification of table formats for use case diagrams.

\* Timeline for discussing the SRS document.

Action Items:

\* Mohammed Yousef Mohammed AbdulKarem will implement predictive
cancellation and rescheduling alerts based on student behavior.

\* Mohammed Yousef Mohammed AbdulKarem will prepare a short validation
survey for student feedback next week.

\* Farah Hanim Binti Mohd Zamri will implement secure login using
multi-factor authentication and AI-driven risk detection for login
attempts.

\* Mohammed Aamena Mohammed AbdulKarem will enhance the goal-setting
feature to suggest realistic goals based on tracked behaviors.

\* Nur Thayiebah Binti Hamdan will ensure that students can view or
delete their data anytime and opt out of AI suggestions if they are not
comfortable.

\* Mohammed Aameena Mohammed Abdulkarem will send the elicitation plan
to Farah Hanim Binti Mohd Zamri by tonight.

\* Mohammed Aameena Mohammed Abdulkarem will work on dividing the SRS
later after finishing the plan and execution.

\* Mohammed Aameena Mohammed Abdulkarem will identify the table format
needed for the use case diagram based on the lecture slide.

Key Questions:

\* What specific AI features should be prioritized for implementation in
phase one?

\* How can the system ensure that AI suggestions are actionable and not
overwhelming for students?

\* What measures will be taken to address incorrect or inappropriate AI
suggestions?

\* Should students be able to turn off specific AI features such as
wellness tips?
