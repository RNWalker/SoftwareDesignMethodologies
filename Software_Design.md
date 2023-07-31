# Software Design Task

**1. What do we mean by coupling and cohesion when discussing structured design?**

In structured design, coupling refers to the depedency of different parts of a system to one another. A tightly coupled system is one with high dependency, meaning that changes in one part of the system can affect other parts, making these systems a challenge to modify. 
Cohesion is how well the compenents inside a system synergise together. High cohesion in a system means the elements comprising that system are well-defined, closely related and contribute to a specific task.
A well designed system will ultimately aim to achieve loose-coupling and high cohesion.

**2. What is the difference between top-down and bottom-up design? Which best describes a function oriented design?**

Top-down design begins with a high-level overview of the system and breaks it down into smaller components, whereas bottom-up design begins with the individual components and assembles them into a more complex system. 
Function oriented design, much like top-down, begins with the overview of the overall function of a programme. It is then broken down into smaller, more manageable components in order to achieve the lower-level details to achieve the function of the programme.


**3. In which design methodology would a class diagram be most useful?**

In object-oriented programming, class diagrams are used to visualise the relationships between modelled entities or abstract concepts.

**4. What are the four pillars of object oriented programming? Give a single-sentence description of each.**

The four pillars of object oriented programming are encapsulation, abstraction, inheritance and polymorphism.

Encapsulation is the grouping of data and methods acting on that data into one class.
Abstraction is hiding all but the most relevant data about an object in order to avoid unnecessary complexities.
Inheritance is creating subclasses that can inherit all the functionality of a previously defined superclass, reducing code redundancy.
Polymorphism is accessing objects of different types through an interface, thus allowing different classes to be treated uniformly and allowing for extensibility. 

**5. What is the strategy pattern? How would its implementation differ between a functional and object oriented system?**

The strategy pattern is a behavioural design pattern that allows a user to change the behaviour of an object by selecting the apporpriate algoirthm dynamically while the programme is running. In an object oriented system, this is achieved by implementing interfaces and classes. In a functional system, strategy pattern is achieved using higher order functions or function pointers, allowing for dynamic function calls.

**6. Imagine your is creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.**

For a flexible and scalable payment system, I would use object oriented design (OOD). With OOD, I could utilise inheritance and polymorphism in order to extend common functionality between classes for specific sectors and implement behaviours through interfaces that treats all the sectors uniformly. For example, a coat may inherit from clothes and a takeaway may inherit from food, but both payments for those items should be processed in a uniform manner. Using a common interface also allows for greater flexibility and extensibility, such that if I decide to enter the market at another sector, that sector could be encoded to interact with the interfaces as the other sectors do, configuring the new sector with the common concepts and functionalities addressing by my existing code. OOD would allow my payment system to adapt to future changes with minimal impact on existing functionality, addressing the needs of the business to evolve and scale. 