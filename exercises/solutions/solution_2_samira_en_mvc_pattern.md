# Introduction and definition of MVC patterns
  The MVC design patterns is also known as Model-View-Controller. It is a common architectural pattern used to design and create an application's interfaces and structure. Also, it is a software architectural pattern for implementing user interfaces. The MVC is an architectural pattern that separates an application into 3 main logical components: the model, the view and the controller. Each of these components are built to handle specific development aspects of an application. MVC is one of the most frequently used industry-standard web development framework to create scalable and extensible projects

  # MVC Component
  There are three MVC components which are,
  -Model: Model classes are used to implement the logic of datat domains. These classes are used to retieve, insert or update the data into the database asociated to it. The model component can either represent the data thatis being transfered between the view and controller components or any other business logic related data. example; a customer object will retrieve the customer information from the database, manipulate it and update it back to the database or use it to render data

  -View: The view component is used for all user interface logic application. ALso, view are used to prepare the interface of an application. By using the interface, users interact with the application. For example, the customer view will include all the user interface componenents such as text boxes, dropdowns etc that the final user interacts with.

  -Controller: Controller classes are used to respomd to the user's requests. Controllers act as an interface between model and view components to process all the business logic and incoming requests, manipulate data using the model component and interact with the views to render the final output. Cotroller classes perform the user requests action. These classes work with model classes and select the appropriate view that should be displayed to the user according to user requests.  Example, the customer controller will handle all the interactions and inputs from the customer view and update the database using the customer model

  # Features of an MVC Pattern
    MVC pattern architecture is basically a 3-layered architecture. It separates the charateristics of application. Its first layer is related to the user input logic, second layer is related to the business logic and third layer is used to implement user interface logc' MVC pattern provides the facility of parallel developmemt. It means that each layer of the application is independent of each other i.e 3 or more developer can work on a single application simultaneously.

# Advantages of MVC Patterns 
- Organizes larrge-size web application
    As there is segregation of the code among the three levels, it becomes extremely east to divide and organize web applications (which are required to be managed by large teams of developers). The major advantageis=f using such code practices is that it helps to find specific portions of code quickly and allows the addition of new functionality with ease.

- Supports assynchronous method invocation (AMI)
   Since the MVC architecture works well with Javascript and its frameworks, it is no surprise that it also supports the use of AMI, allowing developers to build faster loading web applications 

- MVC architecture helps us to control the complexity of applications by diving it into its 3 components 

- MVC use front controller pattern. Front controller pattern handles the multiple incoming requests using single interface (controller). Front controller provides centralised control. We need to configure only one controller in web server instead of many.

# Tools and architecture used in MVC
 There are many tools nd technologies used in MVC which can be used to develop web applications with the help of MVC architecture 

 # Tools
 Visual studio, MySQL server, My SQL workbench, Net beans, Glassfish server 

 # Technologies 
 HTML, CSS, JQUERY, AJAX for designing
Servlet and Javaserver pages used with Net beans 
Enterprise Java beans technologies

# Conclusion
MVC pattern architecture and integrated technologies just like JSP, Servlet and EJB on the platform of J2EE have simplified the development process of web applications. We can make scalable, transparent and portable web application with the help of MVC architecture. MVC architecture provide the concept of parallel development as it divides the logic of application into three layers, so each different developer can work simultaneously on these three 
layers of the same web application. 

First layer of MVC architecture is model which is used to interact with the database. It is basically logic layer of our application which is used to insert, retrieve and update data in the database.Second layer is view which is related to the user interface, through which users interact with our application, how our application will be presented to the users, basically it is used for front end development. Third later of MVC architecture is controller which is used to get inputs from the users. It controls the updates of model object state and data displaying to the users according to user’s inputs. User can request to our application and can get response through controller layer. 