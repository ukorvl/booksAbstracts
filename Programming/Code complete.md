Code complete by STEVE MCCONNELL

--------------------------------------------------------------------Chapter 1

#Software BUILDING not writing, coding or programming#

Consists:
•	Building and debugging
•	Software design
•	Creating a plan of building
•	Testing
•	Integration

Software building is the main chapter of developing, and the main part of a project. Sales, marketing and etc are important, but the software itself is more significant. Project can’t live without a product.
Developer and coder are different specializations. Dev must be able to do more. Dev is more creative. Dev often works not only with code, but with people and very often he must design soft, not only code it.
Devs are the core of the team.


--------------------------------------------------------------------Chapter 2

#METAPHOR#

Metaphor is a very powerful method of understanding and explaining. Metaphor helps you to think more effectively and to understand complicated systems. The history of science is full of discoveries that were made through metaphors.

Metaphor should be sharp, related to real material world, and easy to understand.

Metaphor does not give you an answer. It just explains how to find the answer and how to ask right questions.

We can mix and combine metaphors to look on the subject from different sides and to be more creative and acceptable to innovations.

Metaphor can be dangerous when you are too related to it. It can lead you to incorrect conclusions.

The key metaphors in programming:
•	Literary metaphor of coding
•	Metaphor of a pearl (slow accretion of soft). Incremental approach
•	Building metaphor (like building a house)


--------------------------------------------------------------------Chapter 3

#WORKING WITH CUSTOMERS, PREVIOUS CONDITIONS#

Importance of planning and developing previous conditions
	1.	Define the type of software you want to build
	2.	Planning and defining of preparatory requirements is very important
	3.	Correcting of mistakes and bugs costs mush less at the beginning of the work
	4.	Clients are stupid creatures. It’s extremely important to clearly define requirements at the beginning because they always want to change them and bring some new unreal details to project. Tell them that it will affect price and terms – always works!
	5.	Preparation == risk-off
	6.	Attention to the quality == CONST during all work from start to end
	7.	Define the problem of customer (what he or she really wants??) clearly
	8.	Explain importance of preparatory requirements to colleagues and customer
	9.  Always think about architecture / structure of the project
	10.	Preparation usually takes 10-15% of working on project time

Iterative and serial approaches (best practices) to build software:
Iterative - cyclical work, every cycle contains planning, implementation, checking and adjusting.
Serial (waterfall) - working step by step on each stage. Every stage should be done before next stage can start.


--------------------------------------------------------------------Chapter 4

#BEFORE THE BEGINNING#

Programming in language is worse than programming into language, cause it will restrict you. 
Dont bind yourself with one language.
Think wider than languge frames. Modify loanguage and write your own features and libs if it is needed.

It's radically important to choose language of programming right.
Every language has its benefits and its weaknesses - use benefits of them and avoid weaknesses. 

Its also important to pay attention for methods of software building and patterns. There are to many of them to use in one proj.
So you should make a decision witch of them will be included.

ALWAYS define rules of coding and coding style at the beginning.

--------------------------------------------------------------------Chapter 5

#DESIGNING SOFTWARE (before building)#

The are some typical problems in designing software:
1. Analysing competing technologies of the project and balancing them
2. Design not only features and opportunities but limits of your software too
3. Sometimes software design is heuristic process, don't try to design only logical approach
4. More often than not the problem of the design is a dirty problem (it means that you will truly understand the problem only after building software and not earlier, some problems will appear only after implementation)

We must solve complicated problems with simple methods. Mistakes can be:
	-solving simple problem with comploiated methods (overkill)
	-simple but wrong solution

Levels of software design:
1. System
2. Subsystems - modules and packages. It's very important to define interaction between them and to make them reusable, movable and easy to edit without editing all the system. All the system can not depend on subsystem. Common subsystems: GUI, api.
3. Classes - defining classes and interaction between them, especially their interfaces. One of the most important aspect of OOP is difference betweeen class and object. Class - is a bun backing dish, object - the bun itself.
4. Data and methods - some data and methods can be too complicated and require design
5. Designing methods - defining individual methods

Once again, software design is not determined process, so we should use heuristic methods.

While designing we always work with objects of real world. We must decide which objects are required in our project.
The target is to MINIMISE complexity. Use following working with real objects:
1. Abstarction - is power weapon against real world complexity. Don't copy real objects but use only parameters which are truly needed.
Abstraction tells us: "you can look at this house from bird's eye"
2. Incapsulation - hides all the details. Incapsulation restricts your ability to look at the details of your house. It tells:
"you can not get nearer, look only from afar"
3. Inheritance - helps to group objects. It helps to implement common methods, which every object of some group must have.
4. Hide information and realisation. Class should hide information iside. For example class can have 25 methods, but its interface
should allow access only to 4-5 of them. Interface of a class should be like a top of an iceberg, showing only a little part of it above the water.
5. Always think about future changes. Make classes adaptive and easy to change. New classes, methods and data should not affect old classes.
Design interfaces so that changes inside them don't affect their interactions with other interfaces. Class changes should stay hidden from other classes. Separate elements which look like unstable at the beginning of design.
6. Use best practisies, like design patterns. Don't invent the wheel. Patterns make communication between developers easy. They show possible approaches to solve your problem, its always easier to choose than to invent. 
7. Give every class single responsibility.

Sometimes brute force is needed. If you are in doubt use brute force.

Draw schemes, it's always better to understand and explain with the picture.

Divide and rule! It's easier to work with small parts of code.

"Going up" and "going down" design.
You go up when you first determine specific objects and after that move to abstract classes. It's composmosition strategy.
Going down means working with abstracts first. It is decomposition strategy.

Always try to find balance between coding and designing.

--------------------------------------------------------------------Chapter 6

#CLASSES#
Abstract data is always needed. it's a very powerful instrument in every science. The ability to abstract problem area from very complicated world and solve it is a key to succes.

The key point is hiding realisation. If you work with abstract object you just call it's abstract methods, and this methods are the same for every person who works with it. This makes abstract data multifunctional. All realisation of this methods is hidden inside them. 

Abstract data on all levels of complexity. Just very small and simple needs it. 
Always remember about principle of anonymity - give as little data as it's possible.

Abstraction is a base for class concept.


*Quality class interface* is very important thing.
Perfectly one class should present one abstract data. So it's interface should contain only corresponding methods.

Sometimes you'll see that one part of methods works with one part of data and another part of methods works with the other data. This is a sign that in fact you have two classes and should divide your class.

Think about reverse methods. If you add method "turnOnLights()", then you'll possibly need a method to turn them off.

Minimize access to class methods. If you are disappointed about shoul method be opened of closed, just try to make it closed.

Do not give access to class data, always use getters and setters instead.

*Coupling* - is a strength of bonds between two classes. Always try to minimize coupling between classes.


