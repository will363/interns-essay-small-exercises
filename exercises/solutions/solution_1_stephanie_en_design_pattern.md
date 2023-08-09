## Design Patterns
### Introduction
   Design patterns are models of code that solve classic problems in software design. They are not ready-made code, but rather templates or guidelines that you can use to create your own solutions. 

## Repository Design Pattern
### Explanation of the design pattern
    The Repository Design Pattern is a way of organizing data access logic in a software application. It provides a common interface for accessing different types of data sources. They makes it easier to test your application logic 
### Advantages of using the design pattern
   * It makes testing easier.
   * It separates the data logic from the service logic.
   * It allows for easy swapping of different data stores.
   * It reduces code duplication.
### Disadvantages of using the design pattern
   * It adds an extra layer of abstraction.
   * It can hide the features and capabilities of the underlying data store.
   * It can lead to code duplication or inconsistency

## Dependecy Injection.
### Explanation of the Dependecy Injection
    Dependency injection is a programming technique that allows an object or function to receive other objects or functions that it depends on, instead of creating them itself. This way, the object or function does not need to know the details of how the dependencies are constructed or stored, and can focus on its own logic. 

### Advantages of using the Dependecy Injection
   * It makes testing easier
   * It separates the concerns of constructing and using objects
   * It allows for easy swapping of different implementations of the dependencies
   * It reduces coupling between classes and their dependencies.

### Disadvantages of using the Dependecy Injection
   * It increases the complexity and reduces the performance of the application
   * It hides the features and capabilities of the underlying data store
   * Potential performance issues.

## Observer
### Explanation of the Observer 
    The observer  is a way of organizing the communication between objects that have a one-to-many dependency relationship. It means that when one object (the observable) changes its state, all the other objects (the observers) that depend on it are notified and updated automatically.
### Advantages of using Observer
   * It decouples the observable from the observers.
   * It allows for dynamic registration and deregistration of observers at runtime.
   * It supports broadcast communication.

### Disadvantages of using Observer
   * It can cause memory leaks.
   * It can create performance issues.
   * It can introduce complexity and ambiguity.

## Decorator
### Explanation of the Observer 
The decorator design pattern is a way of adding new functionality to an existing object without modifying its structure or behavior. This pattern is useful for implementing event-driven systems.
### Advantages of using Decorator
   * It decouples the original object from the decorator objects.
   * It allows for dynamic registration and deregistration of decorator objects at runtime.
   * It supports broadcast communication.

### Disadvantages of using Decorator
   * It can cause memory leaks.
   * It can create performance issues.
   * It can introduce complexity and ambiguity.

## Conclusion
    Design patterns are essential in modern backend development as they provide a structured approach to solving common problems as can be seen aboves. it teaches you how to solve all sorts of problems using principles of object-oriented design. 