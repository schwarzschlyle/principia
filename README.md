
# Principia Specifications



## Adviser UI




## Student UI

### Main Page Top Half

Top half of the main page consists of a road map which is a sequential graph view of the tasks. The student can create, delete, or modify the tasks. The tasks are represented as nodes.

Node colors: (Blue) Completed, (Green) In Progress, (Red) Roadblock, (Grey) To-Do

(Insert graph specifications)


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
[Link to Overleaf:]
[Task Description:]

This constitutes the header of the task page. The task page body constitutes of the **Research Journal**. A button named *Add Entry* can be clicked add new entry where the student can type any progress on the task and can paste streenshots on. Upon clicking, it should prompt the student to write a concise description of that entry. When finished, the student can click the *Submit Entry* button which places the entry on the Research Journal with the associated datetime when it was submitted which is inline with the entry description. For example, the journal entry should look like

[12-23-24:13:01] Calculation of the Riemann tensor

(Insert journal entry or screenshots)

[12-26-24:14:21] Calculation of the Ricci tensor

(Insert journal entry or screenshots)

[12-28-24:17:21] Calculation of the Einstein tensor

(Insert journal entry or screenshots)

At the end of each Task Page, there are two buttons: **Verify** which sends a notification to the adviser and **Mark as Roadblock** which also sends a notifcation to the adviser.

## Tabs Sidebar

The sidebar allows the user to switch over different task tabs. Each task tab can be removed from the sidebar with an X button. However, the default Main Page has no X button.



