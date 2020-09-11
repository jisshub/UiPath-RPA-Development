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

  ![Sequence for google search](./screenshots/robot1/image6.PNG 'image')

- next add _Open Browser_ activity to the that sequence.

- give the _Url_ as string

- choose _Browser Type_ as Chrome in Properties window

- next we want to type in to google. for that add _Type Into activity_

  ![open browser](./screenshots/robot1/image6.PNG 'image')

- later select _cityVal_ variable in textbox
  that holds the city name.

  ![Type into](./screenshots/robot1/image5.PNG 'image')

- next have to add _enter_ to search for what typed in search box. for that purpose, add _Send HotKey_ activity

  ![Send HotKey](./screenshots/robot1/image4.PNG 'image')

- finally opens up a weather for typed in city.

  ![Weather Result](./screenshots/robot1/image8.PNG 'image')

#### Note: Shift + f2 to pause the browser screen.

---

## Scrap Data from Google

- use _screen scrapping_ activity - drag abd add _get full text_ activity.

- first get weather condition.

  ![Weather Condition](./screenshots/robot1/image9.PNG 'image')

- later extract the marked text to a variable name _weatherCondition_.

  ![Create variable](./screenshots/robot1/image10.PNG 'image')

- later extract the temperature.

  ![Temperature](./screenshots/robot1/image13.PNG 'image')

## time: 3:10

---
