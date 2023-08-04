# EASSY ON DESIGN PATTERN.

## INTRODUCTION
   Design patterns are reusable solutions to commonly occuring problems in software design and development. They provide  structured approach to solving specific design challenges and promoting code organization, flexibility, and maintainability.

   Design patterns help developers communicate and share best practices for designing software systems. They are like blueprints that can be applied to different scenarios, guiding the way code and components are structured to achieve specific goals. Some well-known design patterns are; observer pattern,singleton,repository etc.

   By using design patterns,developers can create more robust and scalable softtware that is easier to understand, modify, and extend. They have become an essential part of software engineering to improve code quality and promote efficient development practices.

   There are many types of design patterns but we'll focus on 4 which are; observer pattern, decorator pattern, dependency injection, observer, and decorator pattern.

   * Repository design pattern.
        This is a software architectural pattern commonly used in applications that follows the principle of separation of concerns and the single reesponsibility principle. The main purpose of the repository pattern is to abstract the data access layer from the rest of the application. It provides a way to centralize data access logic and encapsulate the interactions with the underlying data storage, such as databases and web services. Here is how it works:

    1. Data access layer: The repository acts as an intermediary between the business logic of the application and the data storage. It provides an abstraction of the data access layer, allowing the application to work with objects and entities without being concerned about the details of how data ia retrieved, stored, or updated.
    2. Encapsulation of data operations; The repository pattern encapsulates all the data operations e.g, (CRUD operations- create,read,update,delete) withn its implementation. This means thst the business logic doesn't directly interact with the data storage, making it easier to manage and maintain.
    3. Centralized data access logic: By having a single repository for each entity or data type, the data access logic is centralized, improving code reusibility and maintainability.
    4. Decoupling and data layer: Using the repository pattern allows you to decouple the business logic from the data layer, making it easier to swicth data storage implementation without affecting the rest of application.
    5. Unit testing: this pattern facilitates unit testing, as you can easily mock or stub the repository when testing the business logic without touching the actual data storage.

    ### Advantages 
    1. Encourages best practices:The pattern can ecourage adherence to the best practices like encapsulation, DRY (don't-repeat-yourself)priciples,and single responsibility.
    2. Improved testability:By abstracting data access, you can easily vreate mock repositories during testing allowing for more efficient and isolated unit testing.
    3. Centralized data access logic: With a repository, all data access logic is centralized, which can simplify maintenance and update.

    ### Disadvantages
    1. Lack of flexibility; In some cases, the repository pattern may not be the best fit, especiallly if the data access logic is straightforward and unlikely to change.
    2. Learning curve: Developers who are not familiar with the pattern might need some time to undrestand and implement it correcly.
    3. Over-enginering: In smaller project, using the repository pattern may be overkill and can add unnecessary  complexity.                                                                                               



* Dependency injection pattern
  This is a design pattern used in software development to achieve loose coupling between components or classes. It allows you to pass dependencies e.g, objects, services to class from the outside rather than creating them inside the class itself.
  By injecting dependencies, classes become more flexible, maintainable, and testable. The dependency injection helps to promote the single responsibility principle and makes it easier to change or extend the behavior of the software without modifying the classes directly.Here is how it works;

  There're 3 main types of dependency injection: 
  1. Setter injection: Dependencies are set through setter methods after the class instance is created
  2. Constructor injection: Dependencies are passed to a class through its constructor when an instance of the class
  is created.
  3. Interface injection: The class implements an interface that defines methods to inject dependencies.

  ### Advantages
  1. Modularity and reusability: By injecting dependencies rather than hard-coding them within classes, components become more modular and can be easily reused in different contexts.
  2. Testability: DI allows easier unit testing, as dependencies can be mocked or replaced during testing, enabling isolated testing of individual components. 
  3. Ease of maintenance: Since dependencies are clearly defined and provided externally, it becomes easier to understand and maintain code, promoting better code organization.

  ### Disadvantages
  1. Complexity; Implementing dependency injection can lead to increased complexity in the codebase, especially in larger projects.writing up dependencies manually can become cumbersome.
  2. Runtime errors: Since dependency injection relies on runtime wiring of dependencies,there is a higher chance of encountering errors at runtime,such as incorrect configuration.
  3. Overhead: Dependency injection can introduce additonal overhead, as it requires creating and managing instances of objects and passing them around.


* Observer pattern
This is a behavioural design pattern used in software engineering. It defines one-to-many dependency between objects, where one object(the subjects) maintains a list of its dependents(observers) and notifies them automatically of any state changes, usually by calling a method on the observers. This allows the observers to update their state accordingly and keep themselves synchronized with the subject.
The observer pattern allows multiple objects to be notifiednand updated when the state of another object changes, ensuring a loosely coupled and flexible communication mechanism between different components in a system. Here's how it works

1. Subject maintains a list of observers.
2. Observers register themselves with the subject to receive updates
3. When the subject's state changes, it notifies all registered observers.
4. Observers receive the update and can react accordingly.


### Advantages
1. Decoupling: It promotes loose coupling between the subject and its observers. Observers can be added or removed without affecting the subject's logic, enhancing flexibility and maintainability.
2. One-to-many relationship: A single subject can notify multiple observers, providing a straightforward way to broadcast updates to multiple parts of the application.
3. Event-driven-behavior; Observers are notified only when relevant changes occur, leading to efficient and targeted updates.

### Disadvantages
1. Accidental uodates: Observers may receive irrelevant updates if the subject broadcasts more information than neccesary.
2. Debugging complexity: The flow of notifications can become intricate, making it harder to debug and maintain the application.
3. Potential performance impact: In scenarios with large number of observers or frequent update, the notification process can introduce overhead and impact performance.


* Decorator design pattern
   The decorator design pattern is a structural design pattern in object-oriented programming. It allows behavior to be added to individual objects dynamically without affecting the behavior of  other objects of the same class.
   In this pattern, you have a base component interface and concrete component classes that implement this interface. Decorator classes also implement the component interface but add additional functionalities. These decorators wrap the concrete components and modify their behavior at runtime, providing a flexible way to extend the functionality of objects.
   In essence, the decorator pattern promotes the principle of"open for extension,but closed for modification, " making it easier to add new features to existing code eithour altering it's structue. Here is how it works

   1. Start a base component interface or class that defines the core functionality
   2. Create concrete component classes that implement the base component interface or class. Decorators have a reference to the base component interface or class.
   3.Create decorator classes that also implement the base component interface or class. Decorators have a reference to the base component and wrap it.
   4. Decorators add functionalities by extending or modifying the behavior of the base component methods.
   5. You can combine multiple decorators to add mulyiple functionalities to the base component in a flexible and dynamic way.


   ### Advantages
   1. Flexibility: it allows you to add or modify the behavior of individual objects at runtime without affecting other instances of the same class.
   2. Reusability: Decorators can also be reused across different objects or classes, reducing code duplication.
   3. Composability; Decorators can be combined to create multiple variations of an object, enabling a wid erange of possible combinations.

### Disadvantages.
1. Overuse: It's essential to use the decorator pattern judiciously, as excessive use can lead to an explosion of classes and make the codebase difficult to manage.
2. Runtime performance: The decorator pattern may introduce a slight overhaed due to the dynamic nature of adding functionalities at runtime.


## ADVANTAGES OF DESIGN PATTERN.
1. Personalization: Custom patterns can be designed to cater to specific tastes and preferences, enhancing the personalized experience for customers.
2. Creativity and expression: Pattern design allows artists and designers to express their creativity and unique stlye through intricate and imaginative patterns.
3. Visual appeal: Well-designed patterns can be visually captivating, making products and designs more attractive and eye-catching

## DISADVANTAGE
1. Complexity: Creating intricate patterns can be time-consuming and require meticulous attention to detail, making the design process more challenging
2. Copyright issues: Copyright infringement can be a concern, as protecting original pattern designs from unauthoris=zed use can be difficult.
3. Overwhelming design: Poorly executed patterns can be overwhelming and clash with other elememts in the design, detracting from the overall visual appeal.



## CONCLUSION.
   Design patterna are essential tools in software development that helps solve common design problems and improve code maintainability,reusability, and flexibility. They provide a structured approach to designing software and allow developers to communicate and share best practices. By applying design patterns,developers can create more robust, scalable and efficient solutions. It's crucial to choose the appropriate design pattern for each specific problem to achieve desired benefits and avoid over-engineering. Overall, understanding and utilizing design patterns can greatly enhance the quality of software projects.