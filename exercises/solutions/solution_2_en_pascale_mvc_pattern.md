# MVC (Model View Controller)

MVC is a pattern in software design commonly used to implement user interfaces, data, and controlling logic. It emphasizes a separation between the software's business logic and display. 
It divides an application into three distinct parts: the model, the view and the controller. Each of these distinct parts has a responsibility in the application.

The three parts of the MVC software design pattern can be described as follows:

Model: Manages data and business logic.
View: Handles layout and display.
Controller: Routes commands to the model and view parts.

## Model

The model defines what data the app should contain. If the state of this data changes, then the model will usually notify the view (so the display can change as needed) and sometimes the controller (if different logic is needed to control the updated view).
It is responsible for managing the database, retrieving and manipulating data, and updating the state of the application. It is generally implemented in the form of properties and the methods necessary to manage the data.

## View

The view defines how the app's data should be displayed. This level is majorly associated with the User Interface(UI) and it is used to provide the visual representation of the MVC model. Typically, this user interface is created from model data.

## controller

The controller contains logic that updates the model and/or view in response to input from the users of the app.

In an MVC application, the view only displays information; the controller manages and responds to user inputs and interactions. For example, the controller handles query string values ​​and passes them to the model, which in turn queries the database using the values.

The controller is responsible for managing the interactions between the user and the application. It receives user requests, queries the model to retrieve the necessary data, and returns that data to the view for display. It is implemented as a series of functions or methods that are called in response to user actions.

##  Advantagesand disadvantages of using MVC design pattern

It makes it easier to manage complexity by breaking down an application into model, view, and controller.
It does not use view state or server forms. The MVC framework is therefore ideal for developers who want complete control over the behavior of an application.
It uses a front controller model that handles web application requests through a single controller. This way, you can design an application that supports a complete routing infrastructure.
It works well for web applications that are supported by large teams of web developers and designers who need a high degree of control over application behavior
Advantages -
1.      Each MVC object has different responsibilities
2.      The development progresses in parallel
3.      Easy to manage and maintain your app code
4.      All classes and object are independent of each other

Disadvantages -
1.      The model pattern is little complex
2.      It is little difficult to use MVC as like modern user interface.
3.      Inefficiency of data access in view 

## conclusion
In conclusion, the MVC design pattern is an architectural pattern widely used in software development. It helps separate an application's concerns into three distinct components, simplifying the application's code and making it easier to maintain. Although it has some disadvantages, the advantages of using the MVC design pattern outweigh its disadvantages. The MVC design pattern is a solid and proven architecture that can significantly improve the quality and maintainability of applications.

