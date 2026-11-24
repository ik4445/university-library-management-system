# Assignment 02
# University Library Management System (LMS)

## 1. Introduction

The University Library Management System (LMS) is a software engineering project designed to improve the management of university library operations. The system will provide an organized way to manage books, students, faculty members, borrowing, returning, reservations, and overdue notifications.

The proposed system will reduce manual paperwork, improve record accuracy, and make library operations more efficient.

### 1.1 Purpose

The purpose of this document is to identify stakeholders, analyze their needs, define functional and non-functional requirements, prepare user stories, and establish acceptance criteria for the University Library Management System.

### 1.2 Project Scope

The system will include:

- Book management.
- Student and faculty membership management.
- Book borrowing and returning.
- Book reservations.
- Overdue book tracking.
- Overdue notifications.
- Basic library reports.

The project focuses on requirements analysis, system modeling, interface prototyping, and documentation. Complete software implementation is not included.

### 1.3 Definitions

| Term | Definition |
|---|---|
| LMS | Library Management System |
| SRS | Software Requirements Specification |
| Stakeholder | A person or group affected by the system |
| User | A person who interacts with the system |
| Administrator | Person responsible for managing the system |
| Librarian | Person responsible for daily library operations |
| Functional Requirement | A service or function the system must provide |
| Non-Functional Requirement | A quality or performance requirement |
| Acceptance Criteria | Conditions used to verify whether a requirement is satisfied |

# 2. Stakeholder Analysis

Stakeholders are individuals or groups who interact with or are affected by the Library Management System.

## 2.1 Identified Stakeholders

The project identifies the following five stakeholders:

1. Librarian
2. Student
3. Faculty Member
4. Library Administrator
5. University Management

## 2.2 Stakeholder Needs Table

| Stakeholder | Role | Needs and Expectations |
|---|---|---|
| Librarian | Manages daily library activities | Add books, update records, issue books, receive returns, and track overdue books. |
| Student | Uses library services | Search books, borrow books, reserve unavailable books, and receive notifications. |
| Faculty Member | Uses library resources | Search, borrow, reserve, and return books. |
| Library Administrator | Manages the system | Manage users, membership records, book records, and system activities. |
| University Management | Supervises library operations | View reports, borrowing statistics, and overdue records. |

## 2.3 Stakeholder Importance

- Librarian: Responsible for daily system operations.
- Student: Main user of library services.
- Faculty Member: Uses library resources for teaching and research.
- Library Administrator: Responsible for system management.
- University Management: Uses reports for decision-making.

# 3. Functional Requirements

Functional requirements describe the operations and services that the system must provide.

| ID | Functional Requirement | Priority |
|---|---|---|
| FR-01 | The system shall allow the administrator to add new books with unique identification numbers. | High |
| FR-02 | The system shall allow authorized staff to update and delete book records. | High |
| FR-03 | The system shall maintain student and faculty membership records. | High |
| FR-04 | The system shall allow members to search for books by title, author, category, or ISBN. | High |
| FR-05 | The system shall allow librarians to issue available books to valid members. | High |
| FR-06 | The system shall record book borrowing dates and return deadlines. | High |
| FR-07 | The system shall allow librarians to record returned books and update their availability. | High |
| FR-08 | The system shall allow members to reserve books that are currently unavailable. | Medium |
| FR-09 | The system shall identify books that have passed their return deadlines. | High |
| FR-10 | The system shall generate overdue notifications for members with late books. | Medium |
| FR-11 | The system shall maintain borrowing and returning transaction histories. | Medium |
| FR-12 | The system shall generate basic reports about available books, borrowed books, and overdue books. | Medium |

# 4. Non-Functional Requirements

Non-functional requirements describe the quality and performance characteristics of the system.

| ID | Requirement | Description |
|---|---|---|
| NFR-01 | Performance | The system should display search results within 3 seconds under normal operating conditions. |
| NFR-02 | Security | Only authorized users should access administrative functions. |
| NFR-03 | Usability | The interface should be simple and understandable for students, faculty, and library staff. |
| NFR-04 | Reliability | The system should maintain accurate borrowing, returning, and book availability records. |
| NFR-05 | Availability | The system should be accessible during the university library's operating hours, provided the required network and hardware are available. |
| NFR-06 | Maintainability | The system should allow authorized administrators to update book and member records without affecting unrelated records. |

# 5. Assumptions and Constraints

## 5.1 Assumptions

1. Students and faculty members can register as library members.
2. Every book has a unique identification number.
3. Members must have valid memberships to borrow books.
4. Every borrowed book has a predefined return deadline.
5. Library staff will maintain accurate book and member records.

## 5.2 Constraints

1. The project has limited development time.
2. The project has limited financial resources.
3. Complete software implementation is outside the project scope.
4. Online operations require computers and internet access.
5. Project activities depend on the availability of team members.

# 6. User Stories

User stories describe system requirements from the perspective of different users.

| ID | User Story |
|---|---|
| US-01 | As a librarian, I want to add new books so that the library catalogue remains updated. |
| US-02 | As a librarian, I want to update book records so that book information remains accurate. |
| US-03 | As a student, I want to search for books so that I can find the books I need. |
| US-04 | As a student, I want to borrow available books so that I can use them for my studies. |
| US-05 | As a faculty member, I want to reserve unavailable books so that I can borrow them when they become available. |
| US-06 | As a librarian, I want to record returned books so that their availability is updated. |
| US-07 | As a student, I want to receive overdue notifications so that I can return books on time. |
| US-08 | As a library administrator, I want to generate library reports so that I can monitor library activities. |

# 7. Acceptance Criteria

Acceptance criteria define measurable conditions that must be satisfied for each user story.

| User Story ID | Acceptance Criteria |
|---|---|
| US-01 | The librarian can enter a book title, author, ISBN, category, and unique book ID. The system saves the record and confirms successful registration. Duplicate book IDs must be rejected. |
| US-02 | The librarian can select an existing book, update its information, and save the changes. Updated information must appear in the catalogue. |
| US-03 | A student can search using title, author, category, or ISBN. Matching results must appear within 3 seconds under normal conditions. |
| US-04 | A valid member can borrow an available book. The system must record the member ID, book ID, borrowing date, and return deadline. |
| US-05 | A faculty member can reserve an unavailable book. The system must save the reservation and display a confirmation message. |
| US-06 | When a librarian records a returned book, the system must update its availability status to available if no other restriction applies. |
| US-07 | When a book passes its return deadline, the system must identify it as overdue and generate a notification for the responsible member. |
| US-08 | The administrator can generate reports showing the total number of books, available books, borrowed books, and overdue books. |

# 8. External Interface Requirements

External interface requirements describe how users and external systems interact with the proposed system.

## 8.1 User Interface

- The system shall provide a login interface for authorized users.
- The system shall provide a dashboard for library staff.
- The system shall provide a book search interface.
- The system shall provide book borrowing and returning forms.
- The system shall display overdue notifications and reservation information.

## 8.2 Hardware Interface

- Desktop computers or laptops will be used to access the system.
- A printer may be used to print library reports.
- Network equipment will support online access.

## 8.3 Software Interface

The proposed system may interact with:

- Operating systems such as Windows or Linux.
- Web browsers such as Google Chrome and Microsoft Edge.
- A database management system for storing library records.
- An email service for sending notifications, if implemented.

## 8.4 Communication Interface

- The system will require an internet or local network connection for online access.
- Communication between the user interface and database should be protected.

# 9. System Constraints and Dependencies

## 9.1 System Constraints

- The system must use unique identification numbers for books.
- Only authorized staff can modify administrative records.
- Members must have valid membership to borrow books.
- Borrowing deadlines must be defined by library policy.
- The project is limited to analysis, modeling, prototyping, and documentation.

## 9.2 Dependencies

- Availability of computers and network infrastructure.
- Accurate book and membership information.
- Defined university library borrowing policies.
- Availability of authorized library staff.
- An email service or notification mechanism for overdue alerts.

# 10. Requirement Priorities

Requirements are classified into three priority levels.

| Priority | Meaning |
|---|---|
| High | Essential requirements for the main library operations. |
| Medium | Important features that improve system functionality. |
| Low | Additional features that may be implemented later. |

High-priority requirements include book management, membership management, borrowing, returning, and overdue tracking.

Medium-priority requirements include reservations, notifications, and basic reports.

# 11. Traceability Matrix

The traceability matrix connects functional requirements with user stories and their acceptance criteria.

| Requirement ID | User Story ID | Acceptance Criteria |
|---|---|---|
| FR-01 | US-01 | Book details are saved and duplicate IDs are rejected. |
| FR-02 | US-02 | Existing book information can be updated. |
| FR-03 | US-04 | Only valid members can borrow books. |
| FR-04 | US-03 | Search results appear within 3 seconds. |
| FR-05 | US-04 | Available books can be issued to valid members. |
| FR-06 | US-04 | Borrowing dates and deadlines are recorded. |
| FR-07 | US-06 | Returned books have their availability updated. |
| FR-08 | US-05 | Reservations are saved successfully. |
| FR-09 | US-07 | Books past their deadlines are identified as overdue. |
| FR-10 | US-07 | Overdue notifications are generated. |
| FR-11 | US-04, US-06 | Borrowing and returning histories are maintained. |
| FR-12 | US-08 | Reports display book and borrowing statistics. |

# 12. AI-Assisted Requirements Review

An AI assistant was used to review the proposed requirements and identify possible ambiguity, omissions, conflicts, and testability issues.

The following suggestions were identified during the review.

| No. | AI Review Suggestion | Decision | Justification |
|---|---|---|---|
| 1 | Every book should have a unique identification number to prevent duplicate records. | Accepted | Unique IDs improve record accuracy and identification. |
| 2 | The borrowing period should be clearly defined. | Accepted | A predefined return deadline is necessary to identify overdue books. |
| 3 | The system should define who can modify book and member records. | Accepted | Access restrictions improve security and prevent unauthorized changes. |
| 4 | Search performance should have a measurable time limit. | Accepted | A 3-second response target makes the performance requirement testable. |
| 5 | The system should include an online payment facility for overdue fines. | Rejected | Online payments are outside the defined project scope. |
| 6 | The system should specify what happens when a reserved book becomes available. | Accepted | This will help avoid confusion in the reservation process. |

## 12.1 Additional Requirement Clarification

The following rules are proposed to improve requirement clarity:

- A book cannot be issued if it is already borrowed or unavailable.
- A member cannot borrow books using an expired or invalid membership.
- A returned book must have its transaction status updated.
- Overdue notifications should identify the book and its return deadline.
- Reservations should be linked to a specific member and book.

# 13. Revision History

| Version | Date | Description | Author |
|---|---|---|---|
| 1.0 | 24-Nov-2026 | Initial SRS document prepared. | M. Jamal Khan |
| 1.1 | 24-Nov-2026 | Stakeholder analysis and requirements reviewed. | Project Team |

