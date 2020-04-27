# CsharpConcept   [![Build Status](https://dev.azure.com/raju1234888/Csharp/_apis/build/status/EzDevPrac.CsharpConcept-Raju%20(1)?branchName=master)](https://dev.azure.com/raju1234888/Csharp/_build/latest?definitionId=5&branchName=master)



### Design Pattern
Design pattern is basically of three types.
A design pattern is a general, reusable solution to a commonly occurring problem within a given context in software design.

Design pattern is basically of three types.

`Creational Design Patterns`
`Structural Design Patterns`
`Behavior Design Patterns`

### Decorator Pattern

Decorator design pattern is one of the **structural design pattern**.As it name specifies it is used to decorate an object with different behaviors.

>  Points to remember 
- Used to load different behavior dynamically with an object .
- One of the structural design pattern.
- Comes handy when you think better way to implement inheritance.
- Follow [Open closed Principle](https://en.wikipedia.org/wiki/Open%E2%80%93closed_principle)
- Easy to modify the classes and it's dependency

### Story Mode:

*This is the story of a Cat named Tom(Many of you may have heard it) a genius programmer. He has a shop of flower bouquet. Tom was designing software for managing his shop and to provide different types of flower bouquet. He was designing his software and writing classes for different types of flower bouquet and during that interval a girl named Terena and his friend Lavanya came and asked do you also decorate these flower bouquet? Tom replied yes we do. And as per the requirement Tom has sold the flower bouquet. Then Tom went on writing the software suddenly this incident struck his mind and he thought that for every type of flower bouquet he needs to add different types of decoration. (**For an example for RoseBouquet there can be n no of decoration such as GlitterRoseBouquet, Paperwrapperbonquet, etc**). So he started thinking that every time he needs to add some new flower or new decoration he needs to modify the overall class. So he started searching on the internet and found help on the book written by [(GoF)](https://en.wikipedia.org/wiki/Design_Patterns). In that he read about decorator patterns which allow him to create an object dynamically with different behavior. He thought to implement this pattern in his software. And he was successful and after that whenever some new decoration comes he just add a class and pass that class behavior to flower bouquet object.*

 

---



### Singleton Pattern

Singleton design pattern is one of the **creational design patterns**. As its name specifies it only be **instantiated** only once. It is useful when the following cases arise.

- When only one instance of a class is created.
- Provide a global access point to this instance.

 **A simple flow of Score calculator in different cases while playing games. I have a `Runningclass` named `Trackscore` and a `killingclass` name `KillScore`. And a `ScoreManager class` which will only create a single instance and provide global access to manage all score during gameplay.**
 
![Flow diagram](https://gitlab.com/vr.srinidhi/retailplusrota/-/wikis/uploads/d103afe7da75dec83b9af9480dd51093/SingletonPattern.png)


*Here is the simple example go play with it [EagerInitilization](https://github.com/EzDevPrac/CsharpConcept-Raju/tree/master/EagerInitilization) and [LazyInitialization](https://github.com/EzDevPrac/CsharpConcept-Raju/tree/master/LazyInitialization)*

---


### Facade Design Pattern.

Facade Design Pattern is part of the **structural design pattern** family. 
1. It is used to simplify the interaction process.
2. Subclass are independent classes.
3. Facade has refrence to these class.
4. Subclass don't have refrence to facade class.
5. Make easierr to create to subclasses due to loose coupling between the subclasses.
6. Act as entry point for each subclasses.

**Go and read this you will enjoy it and can easily grasp the idea behind facade design pattern.**


> Story mode.\
>**For eg...**

>Raju is trying to create an e-commerce website. He finds that many actions are performed by the buyer or the client in this short interval of time. In that short interval a client has to make an order, make payment and wait for the delivery he thinks.<br/>

**These are in general even many more services that are performed during this time.**

>He created class of three services `PaymentService`, and `InventoryService` and linked these with the MainController class. 
After some time he finds that he needed one more subclass ShippingService for delivery status. So he created and linked with the other classes. But he finds that it was very disturbing because of the tight coupling of the classes with each other. 

**Here the client directly interacts with the subclasses and every other classes are tightly coupled.**

 >Every time he do some changes he has to alter every class. 
 
**And to solve this problem facade design pattern is introduced. It simplifies the complexity**.

>After some time he called his friend Srini and explained everything. Srini told him to go through the Facade Design Pattern. So he started looking through the pattern. After some time he was astonished that these problems can be easily solved using this pattern.

**And to solve this problem facade design pattern is introduced. It simplify the complexity. In other sense every service class such as payment, inventory availability,
delivery status will independent. These classes are linked to the facade class. Facade has a reference to every subclass but the subclass don't have a link to the facade.**

>So he created an interface named IOrderServiceFacade. And he implemented that in another class called facade. This facade class has reference to every other subclasses.

**The user will interact with facade class and then the facade class will interact with other subclasses such as inventory, delivery, payment etc. **
  
>So every time client makes an interface with facade class and this class make communicates with every other subclass. Now he doesn't need to change every other subclass to create new subclasses.


### Simple Class Diagram Of facade pattern Implementation.


![FascadePattern](https://gitlab.com/vr.srinidhi/retailplusrota/-/wikis/uploads/b1f8717becfa80ad883f1fbb3a8dfeba/FascadePattern.png)

Go Checkout and play with it [Simple example](https://github.com/EzDevPrac/CsharpConcept-Raju/tree/master/Facade)

---


### Builder design pattern.

 **Builder design pattern which is one of the Creational Design Patterns. Builder design pattern is used to create complex object**.

>>>
The builder pattern allows you to enforce a step-by-step process to construct a complex object as a finished product. In this pattern, the step-by-step construction process remains same but the finished products can have different representations.
>>>
**An example of builder design pattern is given below.**

Checkout and play with it [Simple example](https://github.com/EzDevPrac/CsharpConcept-Raju/tree/master/Builder)


