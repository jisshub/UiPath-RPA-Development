# UiPath Tutorials

## Activities

- r the building blocks of any automation.
- an activity replicates to manual task that v perform on our computer.

- Check RPA Samples

[RPA Samples](https://www.rpasamples.com/)

- choose unicorn name generator

- back to UiPath studio - blank project -

- Add an activity called _input dialog_
  ![Input Dialog](./screenshots/image1.png 'image')

- create variable to store user name label
  ![Create Variable](./screenshots/image2.png 'image')

- assign Result to the variable name.
  ![Add Result](./screenshots/image3.png 'image')

---

- next thing is to automate the browser

- for that choose _Open Browser_ activity.
- set browser type to Chrome
  ![Set Browser type](./screenshots/image7.png 'image')

from list, then add _Type Into_ activity.

- give _userName_ variable where v store value to the text box.
  ![Type Into Activity](./screenshots/image4.png 'image')

- next add _click_ activity for button.
  ![Click Button Activity](./screenshots/image5.png 'image')

- next add _get text_ activity for unicorn value generated.

- so create new _variable_ for this.

- assign that variable to _Output_ Value of that activity.

---

- store unicorn name to a _text file_.
- for that add _write text file_ activity.
  ![Write Text File Activity](./screenshots/image6.png 'image')

- file will be saved in _project folder_

- Click _Debug File_ or F6.

---
