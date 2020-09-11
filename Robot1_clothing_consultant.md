# Robot 1: Building Clothing Consultant

## Aim: Ask for city and suggest a clothing depending on weather in city.

## Input Dialog

- when v start a project - add a container to the workflow. a container
  can be a **sequence** or **flowchart**. here v use sequence.

- here robot asks for city name, so to get input from user, use **Input Dialog**.

![Input Dialog](./screenshots/robot1/image1.PNG 'image')

- after Debug

![Result](./screenshots/robot1/image2.PNG 'image')

- next v have to create a variable to assign the city value v input.

![Variable](./screenshots/robot1/image3.PNG 'image')

- so here use _cityVal_ as variable to hold city.

---

## open browser and search

- here v scrap weather data from google.

- first add a container for instance a, _sequence_.

  ![Sequence for google search](./screenshots/robot1/image7.jpg 'image')

- next add _Open Browser_ activity to the that sequence.

- give the _Url_ as string

- choose _Browser Type_ as Chrome in Properties window

- next we want to type in to google. for that add _Type Into activity_

  ![open browser](./screenshots/robot1/image6.jpg 'image')

- later select _cityVal_ variable in textbox
  that holds the city name.

  ![Type into](./screenshots/robot1/image5.jpg 'image')

- next have to add _enter_ to search for what typed in search box. for that purpose, add _Send HotKey_ activity

  ![Send HotKey](./screenshots/robot1/image4.PNG 'image')

- finally opens up a weather for typed in city.

  ![Weather Result](./screenshots/robot1/image8.jpg 'image')

> Note: Shift + f2 to pause the browser screen.

---

## Scrap Data from Google

- use _screen scrapping_ activity - drag abd add _get full text_ activity.

- first get weather condition.

  ![Weather Condition](./screenshots/robot1/image9.jpg 'image')

- later extract the marked text to a variable name _weatherCondition_.

  ![Create variable](./screenshots/robot1/image10.jpg 'image')

- later extract the temperature.

  ![Temperature](./screenshots/robot1/image13.jpg 'image')

- finally close the chrome tab. use _close tab_ activity

- next output the scrapped data in a window, so use _writeLine_ activity .

  ![Final Output](./screenshots/robot1/image15.jpg 'image')

> Note: **Environment.NewLine** used to move to new line

---

## Flowchart

### Robots to make decision based on flowcharts.

> flowcharts are used when v want to make business decisions.

> add flowchart activity

![Final Output](./screenshots/robot1/image16.jpg 'image')

> later add a _flow decision_ activity which suggest a cloth if temperature is too cold and also suggests one if temperature is hot. also if temperature is b/w hot and cold, we suggest another cloth, for that v connect the start node with _flow decision_.

![Flow Chart Basic Structure](./screenshots/robot1/image17.jpg 'image')

- Activities used:
  - Flowchart (1)
  - flow decision (2)
  - Assign (3)

---

## Using Conditions

- next add constraints to flow decision elements in flow chart.

- click on flow decision where v want go set the condition,

  ![Flow Decision Constraint](./screenshots/robot1/image20.jpg 'image')

- select _condition_ property from Properties panel.

  ![Flow Decision Constraint](./screenshots/robot1/image19.jpg 'image')

---

## Assigning Values to Variables

- here v assign values to variable _outfitSuggestion_

![Assigning Values](./screenshots/robot1/image21.jpg 'image')

---

## Display Weather, Temperature, Suggestion in MessageBox

---
