
# Principia Specifications


## Frontend

### Adviser UI




### Student UI

**Main Page**

Top half of the main page consists of a road map which is a sequential graph view of the tasks. The student can create, delete, or modify the tasks. The tasks are represented as nodes.

Node colors: (Blue) Completed, (Green) In Progress, (Red) Roadblock, (Grey) To-Do

(Insert graph specifications)


Beside the roadmap, there is a *Verification* status checkbox. If it is already adviser-verified, the checkbox is checked.
If it the roadmap is not yet verified, a button appears which sends verification request to the adviser. If the adviser confirms the roadmap verification, the checkbox is checked. Every modification on the roadmap removes the **Verified** status.



## Backend