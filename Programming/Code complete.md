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
Design interfaces so that changes inside them don't affect their interactions with other interfaces. Class changes should stay hidden from other classes. Separate elements which look like unstable at the beginning of design. You can use Adapter pattern for example to make one outcoming format of data, which another classes can use with one method without cheking this data.
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

**EVERY class should have it's own main purpose.**


*Quality class interface* is very important thing.
Perfectly one class should present one abstract data. So it's interface should contain only corresponding methods.

Sometimes you'll see that one part of methods works with one part of data and another part of methods works with the other data. This is a sign that in fact you have two classes and should divide your class.

Think about reverse methods. If you add method "turnOnLights()", then you'll possibly need a method to turn them off.

Minimize access to class methods. If you are disappointed about shoul method be opened of closed, just try to make it closed.

Do not give access to class data, always use getters and setters instead.

*Coupling* - is a strength of bonds between two classes. Always try to minimize coupling between classes.


Do not include too much data to one class. Orient yourself to 7-10 data objects in one class. If there is too much data divide this class.

Child class must be just more specific version of parent class. In a nutshell child must be kind of parent. You should have an ability to say: 'child is parent'. Parent class determines all its inheritors, so it's radically important to design parent class very precisely. If child don't fit very well, it's better to remake parent or if it is not possible not to use inheritance at all.

Remember Barb Liscov principle - all parent methods should exist in children classes and be invocable without any differences.

*Make sure that you inherit only what you need.* Inherited methods can be: abstract redefined method (child inherits only method's interface, not implementation), redefined method (inherits interface and implementaion and can redefine it), non-redefined (inherits all but can not redefine). So don't inherit too much. If you need only implementation but not interface, use including but not inheritance.

Don't use more than 6-7 levels of inheritance. Otherwise it will be increasing of complexity but not managing of it.

Don't be fan of inheritance because sometimes it leads to growing of complexity. 

Some simple rules of useing inheritance:
		1. If some classes have common data but not methods don't use inheritance. Just create a common object and include it into them.
		2. If some clases have the same behaviour but not data, make them children of one base abstract class, which will define this methods.
		3. If some classes have common behaviour and data olso use inheritance and define data and methods in parent class.
		4. Use inheritance when you want to define interface by base class and including when you want to manage interface by yourself.


*Main reasons to create a class*
You can create class for every object of the real world, abstarct class for abstract object which does not exist, like Shape (with real children like Square).

Decreasing complexity is the main reason for creating a class, because class helps to hide data and implementation inside.

Reusing of code is the other reason to create classes, because classes make your code easy to reuse.

Avoid creating classes which contain little data and big methods, with names like StringBuilder or DataInitialization, sometimes it's better to transform them into methods.




--------------------------------------------------------------------Chapter 6

#METHODS#
There are some criteria to check your methods:
1. Method should have understandable name
2. M should be described in description
3. If it is possible M should be pure function
4. M should have one main purpose (if it is not - divide method)
5. M should take less arguments (5-7 is enough)
6. M should have strength (should have high cohesion) - it means M should not solve different tasks

Methods is the most effective way to solve problem of complexity of your code.
Methods prevent repeating of code.
Methods help to refactor your code (it is all settled in one place).
Methods help to read and understand code
Methods are reusable

*Create even simple methods of three or four strings of code. It may be helpful in future*

Method can be functional (to do some actions), organizing (to invoke group of another methods), event handlers (to handle different cases of some data and invoke the corresponding methods)

*Naming*
Names of methods should clearly describe their role. Avoid abstract names like DealWithOutput(), be clear.
If you can't clearly describe what this method do in it's name, this method is corrupted and you need to refactor it. 

Describe in the name what this function returns.

Use antonyms (because they are dramatically clear) like open/close, get/set, insert/delete, show/hide.

*Length* of method is olso some kind of problem. Steve recommends to limit them with 50-60 strings of code. In special cases method can contain about 180-200 strings of code but ot more. 




