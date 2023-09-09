# TravelTimeEstimation
Second module project - IT Coding for Data Science - instructor: Dr. Pozzi

### Student
- Full Name: Migliori Luca
- StudentID: 52058800
- email: luca.migliori01@icatt.it

### Introduction
This work aims at designing a tool to estimate the travel time between two points by **car**, based on the route conditions such as types, surfaces and distances in the route. The tool makes use of several APIs, specifically: the openrouteservice API (providing encoded route, details and instructions), the TomTom API (providing traffic conditions) and the OpenStreetMap API (providing the coordinates of the starting and destination points). The tool is designed to be used in a Jupyter Notebook environment, and it is divided in <u>three main sections</u>:
- The first one is the **input section**, where the user is asked to provide the starting and destination addresses, as well as the language of the instructions.
- The second section is the **route section**, where the route is calculated and the map is created.
- The third section is the **analysis section**, where the route is analyzed, and the travel time is estimated by three different models.

### Description
The use is quite simple, the only informations requested are the addresses of starting and destination point and the fuel consumption of the car to get a useful information on the fuel amount needed for that specific route. A step by step explanation is anycase provided.

### Conclusions
In the notebook are listed some conclusions at the end, the results of the tests mentioned can be found in the "Regression tests.xlsx" file already present in the repository.

### Possible Improvements
The development at this stage is limited by time constraints but future improvements are possible, here some key points:
- The tool is currently based only on car travel, but it may also be possible to analyze other types of modes, such as bicycle and walking, both of which are suitable for planning both bicycle and walking trips.
- Regression analysis at this stage is based on the current route, splitting the train trip and test sample according to the 80/20 rule; lack of more data may be a source of inaccuracy in model predictions. One way to increase the amount of data could be to create a database in which, at each simulation, travel data is added at the test stage and used to train the models.
