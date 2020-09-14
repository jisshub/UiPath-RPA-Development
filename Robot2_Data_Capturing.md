# Data Capturing Robot

## Web Data Capturing Robot

- Aim: Adding Personal data tp a crm site automatically using a robot.

## Desktop Data Capturing Robot

- Aim: to fill a CRM app using a robot.

- There is a parallel activity that executes both robots simultaneously(run 2 at same time).

---

## Creating data desktop data capturing robot.

- Create 2 more xaml file. one for web data capturing, one for desktop data capturing

![Xaml Files](./screenshots/robot2/image1.jpg 'image')

---

## Read Data from excel spreadsheet

- create a **Sequence** activity first
- later add an **Excel Application Scope** activity.
- then add **Read Range** activity of **Excel** library inside the **Excel Application Scope**.

  ![Excel Application Scope, Read Range](./screenshots/robot2/image2.jpg 'image')

- then store the sheet to a variable called _customerData_.

![DataTable](./screenshots/robot2/image2.jpg 'image')

---

## Excel Application Scope Properties

> it opens up a workbook and provides scope for this excel activities. when the execution of this activity ends, the workbook and excel application r closed.

- next we have to open browser and navigate to url, use _open browser_ activity.

![open browser](./screenshots/robot2/image4.jpg 'image')

- make it **private**

--

## While loop to loop thru each line in sheets

- add a while loop activity under **open browser** activity

  ![Write Line 2](./screenshots/robot2/image5.jpg 'image')

- add an Assign activity in the Body for creating **rowNumber** variable which acts as Counter.

  ![Assign activity](./screenshots/robot2/image9.jpg 'image')

- assign a default value 0 to the same.

- set the condition for looping.

  ![Condition](./screenshots/robot2/image10.jpg 'image')

- _customerData.Rows.Count_ equals total rows in customerData.

- also can add a write line activity to see the row numbers v looped thru.

### final result

![While Condition](./screenshots/robot2/image11.jpg 'image')

---
