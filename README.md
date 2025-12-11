<div align="center">
  <img src="assets/o6u-logo.jpeg" alt="O6U Logo" width="150" height="auto" />
  <br><br>
  <h1>Library Management System</h1>
  <h3>Software Engineering 1 (Practical)</h3>
  <p><strong>Academic Year:</strong> Egypt 2025/2026</p>
</div>

---

## Team Members

| Student Name | Student ID |
| :--- | :--- |
| **Bassem Said Mahmoud Abdo** (باسم سعيد محمود عبده) | 23015282 |
| **Mahmoud Ragab Saleh Moussa** (محمود رجب صالح موسي) | 23016221 |
| **George Nasser Seif** (جورج ناصر سيف) | 23014881 |
| **Adham Tarek Ahmed Mohamed** (أدهم طارق أحمد محمد) | 23014791 |

---

## Project Overview

### Problem Definition
Current manual processes in university libraries often lead to inefficiencies. Librarians struggle with tracking physical inventory, calculating overdue fines manually leads to human error, and verifying student membership status across different departments is time-consuming.

### Solution Description
We have designed a Library Management System (LMS) to automate these core workflows. This system acts as a bridge between the Librarian, the Member (Student), and the database. It handles the lifecycle of a book from the moment it is added to the inventory, through the borrowing process, and finally its return or reservation.

---

## System Requirements

Based on our analysis, we have defined the following requirements which are represented in our UML diagrams.

### Functional Requirements
1.  **Authentication & Membership:** The system must verify if a student is currently enrolled and eligible for a library card before creating a profile.
2.  **Inventory Management:** Librarians must be able to scan ISBNs to add new titles or update the copy count of existing books.
3.  **Borrowing Logic:** The system must validate that a member has no overdue fines and has not exceeded their borrowing limit before issuing a book.
4.  **Returns & Fines:** Upon return, the system must automatically calculate fines based on the return date and update the book status to "Available" or "On Hold" (if reserved).
5.  **Reservation System:** Members should be able to place a hold on books that are currently checked out.

### Non-Functional Requirements
*   **Accuracy:** Financial calculations for fines must be precise.
*   **Data Integrity:** The system must prevent duplicate member accounts.
*   **Usability:** The interface should provide clear feedback (e.g., "Book Not Found" or "Account Terminated").

---

## Diagrams

Per the project requirements, we have created Activity and Sequence diagrams to visualize the system logic. These files are organized in the repository folders linked below.

### Activity Diagrams
You can view the workflow logic for specific functions in the **[diagrams/activity/](./diagrams/activity/)** folder.

*   **Add New Book:** Shows the flow of scanning an ISBN, checking the database, and updating records.
*   **Borrow Book:** Details the decision process for loaning a book (checking limits and availability).
*   **Return Book:** Illustrates the logic for accepting returns and calculating fines.
*   **Membership Registration:** The process of verifying student data with external systems.

### Sequence Diagrams
You can view the object interaction details in the **[diagrams/sequence/](./diagrams/sequence/)** folder.

*   **Main System Sequence:** A comprehensive diagram covering the full borrowing lifecycle. It details the messages passed between the Member, Librarian, System, and Database entities (Book, LoanTransaction, Fine, MemberAccount).

---

<div align="center">
  <p>Submitted to the Faculty of Computer Science</p>
</div>
