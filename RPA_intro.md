# What is RPA

- Robotic Process Automation(RPA) is a technology which allows a computer program or robot to replicate manual process done by human in an automated fashion.

- for instance, like humans robots can open emails, log into application, read db, collect data, fill in forms and perform calculations.

- use of RPA in banks r
  payment processing, invoice management, reporting, reconciliation.

- top 3 RPA tools are _blueprism_, _UIPath_, _Automation Anywhere_

---

# Building First Robot in UiPath

Aim - build a robot that writes some text to notepad.

- whenever v build a robot, put it in a container.

- first add a sequence to the main window

- later add open application activity to the sequence.

- open notepad

- click _indictive window on screen_

- point to notepad.

- add _type into_ activity to _open application_ activity.

- click _indictive window on screen_

- point to notepad typing area.

- give string value to textbox in double quotes.

- save and debug robot.

- text will be written to notepad automatically.

  ![first Robot](./screenshots/image10.png 'image')

---

# RPA process candidate selection

![Robot Candidates](./screenshots/image11.png 'image')

- **Repetitive** : process is predictable. repeat more than once. more repetitive the process, better the rpa

- **Rules Based**: means process process is based on _if then_ rules.

- **Structured Inputs**: inputs that r accessible without human interventions. rg: csv, excel table.
  more structured the input is, better the rpa

- **Structured Output**: more structured the o/p is, better the rpa.

- **total volume**: rpa is valuable if total volume or no of transactions of the tasks r higher.

- **off hour processing**: machine can run process without become inefficient or ineffective. more time to do a process, process is better for rpa.

- **error prone**: the more prone to human error, the better for rpa.

- **duplicate data** : more duplicate data is, process is better for rpa.

- **process stability** : if process changes frequently , more updates have to be made to the robot, ongoing robot maintenance can be expensive. the more process stability, the better for RPA.

- **quick development**: the amount of time required to build the robot, quicker the development time, the better for RPA.

---