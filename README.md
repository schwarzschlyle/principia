
# Principia App Specifications



## Student UI

### Main Page Top Half

Top half of the main page consists of a road map which is a sequential graph view of the tasks. The student can create, delete, or modify the tasks. The tasks are represented as nodes.

Node colors: (Blue) Completed, (Green) In Progress, (Red) Roadblock, (Grey) To-Do

In this section, there is an Add Task button. When clicked, it should prompt the user the following:

[Task Name]
[Link to Overleaf]
[Task Description]
[Task Prerequisite/s]

Then, based on the task prerequisites, it should generate a clickable graph representation of the tasks. Depending on that graph view, a logic should decide if is in progress (meaning, no prerequisite or the prerequsites are completed) or To-Do (prerequisites are still in progress.)



Beside the roadmap, there is a *Verification* status checkbox. If it is already adviser-verified, the checkbox is checked.
If it the roadmap is not yet verified, a button appears which sends verification request to the adviser. If the adviser confirms the roadmap verification, the checkbox is checked. Every modification on the roadmap removes the **Verified** status.


### Main Page Lower Half

Lower half is divded into three list views:

**Accomplishments** (leftmost) lists the set of tasks marked as Completed. This contains the task ID and the task name which is clickable and redirects you to that task page.

**In Progress** (center) lists the set of tasks marked as In Progress. This contains the task ID and the task name which is clickable and redirects you to that task page.


**Roadblocks** (rightmost) lists the set of tasks marked as In Roadblock. This contains the task ID and the task name which is clickable and redirects you to that task page. For each task, it contains a `Consult` button which sends that task to the adviser. If the adviser resolves the task roadblock, this task gets removed from the Roadblocks and marked as In Progress.


### Task Page

When the user clicks on a task node either from the road map graph view of the top half of the main page or any of the task list on the bottom half of the main page, that specific task page will be opened. The task page will show the following task descriptions:

[Task Name]
[Status: {In Progress, Completed, Roadblock}]
[Task ID: ]
[Task Prerequisite/s]
[Link to Overleaf:]
[Task Description:]

This constitutes the header of the task page. The task page body constitutes of the **Research Journal**. A button named *Add Entry* can be clicked add new entry where the student can type any progress on the task and can paste streenshots on. Upon clicking, it should prompt the student to write a concise description of that entry. When finished, the student can click the *Submit Entry* button which places the entry on the Research Journal with the associated datetime when it was submitted which is inline with the entry description. For example, the journal entry should look like.

[12-23-24:13:01] Calculation of the Riemann tensor

(Insert journal entry or screenshots)

[12-26-24:14:21] Calculation of the Ricci tensor

(Insert journal entry or screenshots)

[12-28-24:17:21] Calculation of the Einstein tensor

(Insert journal entry or screenshots)

At the end of each Task Page, there are two buttons: **Verify** which sends a notification to the adviser and **Mark as Roadblock** which also sends a notifcation to the adviser. After clicking either button, it should prompt the student again to verify that action as it could not be undone and states that the adviser will get notified.

### Tabs Sidebar

The sidebar allows the user to switch over different task tabs. Each task tab can be removed from the sidebar with an X button. However, the default Main Page has no X button as well as the Consultation Calender which will be specified later.

### Consultation Calendar


This calendar is shared by both students and adviser. The calendar is a weekly calendar from Monday to Friday from 6:00 AM to 6:00 PM at 30 minute increments per block where the student can book a consulation. The adviser has the option to block out that schedule and write a brief description to the blocked out timeblock shading it with a color of his choice. The student's can also use the consultation calendar where they can click on the time block and click on a **Schedule Consultation** button. If the adviser confirms the consultation booking, The student's name gets marked on that time block. When the adviser hovers on that booked timeblock, he see that student's Roadblocks and Accomplishments. The other students should not be able to see this when they hover. This tab could not be closed from the sidebar.



## Adviser UI

The adivser's main page center part is constitutes of three parts. The top most is the **Pending Verifications** section. The center page is the **Consultation Calendar** section and the bottom page is the **Research Activity** section. The left part of the page includes the sidebar while the right part of the page constitutes the Journal Entries section.

### Pending Verifications

This top section is divided into two parts. The left part is the Roadblocks section while the right part is the Accomplishment Verification. These constitute clickable lists of tasks after the student clicks either **Verify** or **Mark as Roadblock** for each task page. If the user clicked **Verify** this adds that task to the Adviser's list of Accomplishment Verifcation. Same with **Mark as Roadblock** which gets adds to the Adviser's list of Roadblocks.


### Consultation Calendar

This calendar is shared by both students and adviser. The calendar is a weekly calendar from Monday to Friday from 6:00 AM to 6:00 PM at 30 minute increments per block where the student can book a consulation. The adviser has the option to block out that schedule and write a brief description to the blocked out timeblock shading it with a color of his choice. The student's can also use the consultation calendar where they can click on the time block and click on a **Schedule Consultation** button. If the adviser confirms the consultation booking, The student's name gets marked on that time block. When the adviser hovers on that booked timeblock, he see that student's Roadblocks and Accomplishments. The other students should not be able to see this when they hover.



### Research Activity

On the bottom part of the Main Page of the adviser, there is a bar graph view of each student's activities which correspond to the count if verified accomplishments. The adviser can sort, or datetime filter this bar graph.


### Student List

This is simply a list of students. When clicked, the adviser has the access to the student's main page as well as the tasks when clicked which adds as new tab. However, the adviser could not modify any task.

### Sidebar

This is also where the adviser can switch over tabs. The adviser has two default pages which can't be closed: The Main Page and the Student List page. When the adviser clicks on the any task of the student, it adds a tab to the sidebar with each task having an X button.