# TaskFlow - Követelmények
## Funkcionális követelmények
### FR-01 - Új feladat létrehozása
**Description:**

As a team member, I want to create a new task so that the work to be done can be tracked in the system.

**Acceptance criteria:**

Given that the user is viewing a project, when the user creates a task with the required data, then the new task appears in the project's task list.
### FR-02 - Feladat státuszának módosítása
**Description:**

As a team member, I want to change the status of a task so that the current progress of the work can be tracked.

**Acceptance criteria:**

Given that a task already exists, when the user changes its status, then the task is displayed with the newly selected status.
### FR-03 - Felelős hozzárendelése feladathoz
**Description:**

As a team member, I want to assign a team member to a task so that it is clear who is responsible for completing it.

**Acceptance criteria:**

Given that a task and a team member exist, when the user assigns the team member to the task, then the selected team member is displayed as the assignee of the task.
### FR-04 – Megjegyzés hozzáadása feladathoz
**Description:**

As a team member, I want to add a comment to a task so that I can share information about the task with other team members.

**Acceptance criteria:**

Given that a task exists, when the user adds a comment to the task, then the comment is displayed on the task with its author.
### FR-05 – Feladatok listázása
**Description:**

As a team member, I want to view the tasks of a project so that I can see what work needs to be done.

**Acceptance criteria:**

Given that a project contains tasks, when the user opens the project's task list, then all tasks belonging to the project are displayed.
### FR-06 – Címkék kezelése
**Description:**

As a team member, I want to assign labels to a task so that tasks can be categorized and identified more easily.

**Acceptance criteria:**

Given that a task and a label exist, when the user assigns the label to the task, then the selected label is displayed on the task.
## Nem funkcionális követelmények
### NFR-01 – Teljesítmény
**Description:**

The system shall display the task list within 2 seconds under normal operating conditions.

**Acceptance criteria:**

Given that a project contains up to 100 tasks,
when the user opens the project's task list,
then the task list is displayed within 2 seconds.
### NFR-02 – Biztonság
**Description:**

The system shall store user passwords using a secure password-hashing algorithm and shall never store passwords in plain text.

**Acceptance criteria:**

Given that a user registers with a password,
when the system stores the user's credentials,
then only a securely generated password hash is stored, and the original password is not stored in plain text.
### NFR-03 – Megbízhatóság
**Description:**

The system shall reliably preserve successfully saved task data so that it remains available after the application is restarted.

**Acceptance criteria:**

Given that a task has been successfully saved,
when the application is restarted and the user opens the task list,
then the saved task is still available with its previously saved data.
### NFR-04 – Használhatóság
**Description:**

The system shall provide a clear and consistent user interface so that team members can easily identify task statuses and available actions.

**Acceptance criteria:**

Given that a user opens a task,
when the task details are displayed,
then the current status is clearly labeled and the action for changing the status is identifiable without additional instructions.
### NFR-05 – Böngészőkompatibilitás
**Description:**

The system shall support the latest stable versions of Google Chrome, Mozilla Firefox, and Microsoft Edge on desktop computers without requiring additional browser plugins.

**Acceptance criteria:**

Given that the user opens the application in a supported browser,
when the user views the task list and creates a new task,
then both functions work correctly without browser-specific errors.
### NFR-06 – Adatvédelem
**Description:**

The system shall follow the principle of data minimization by collecting only the personal information necessary for user account management and task assignment.

**Acceptance criteria:**

Given that a new user registers in the system,
when the registration form is displayed,
then only the username, email address, and password are required, and no unrelated personal information is requested.
