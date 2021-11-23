# Polymorphism & Composition Homework - Quiz

# Polymorphism

**1. What does the ___word___ 'polymorphism' mean?**

* Something being of more than one form. 

**2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.**

* In this context, polymorphism means that an object can be of many types and that their behaviour can change according to the type they are called with.  
An example in Java is that every class inherits from the Object class, so instances of that class are both of type Object and of their class type.


**3. What can we use to implement polymorphism in Java?**

* We can use use inheritance and interfaces. 
* @Override to alter inherited methods.  

**4. How many 'forms' can an object take when using polymorphism?**

* There isn't a limit to the number of forms that an object can take. 

**5. Give an example of when you could use polymorphism.**

* We could use it to give customized behaviours to sub-classes.  For example, we could have a Magazine class and Newspaper class that are both sub-classes of a ReadingMaterials class. Magazine objects would be 
of type Magazine and ReadingMaterials whilst Newspaper would be of type Newspaper and ReadingMaterials.
In ReadingMaterials, we could have a printFrequency() function.  Both the Magazine and Newspaper class will have this function as they are both 
of type ReadingMaterials as well as Magazine or Newspaper, and they each apply it differently.
For example, the Magazine could return "Print once a month" whilst the Newspaper could return "Print daily".

* You could also use it to include objects of different types in an ArrayList, by using either an interface or parent-class that is common between 
each of the objects.



# Composition and Aggregation

**6. What do we mean by 'composition' in reference to object-oriented programming?**

* Where one object needs an instance of an object from a different class when it is being constructed.  So the object being composed is dependent on the other object.

**7. When would you use composition? Provide a simple example in Java.**

* You could use it when you want to build something but extract away a layer of the complexity from it.  For example,an object of type Human could be composed of a Heart object and a Lungs object.  If the Human object doesn't include both of these objects then it can't exist. 

**8. Give a difference between composition and aggregation?**

* In composition, the composed class can't exist without the other class and in aggregation, the classes can exist independently. 

**9. What is/are the advantage(s) of using composition/aggregation?**

* It is an example of abstraction, so keeping layers of complexity seperated. That is, a class that uses composition or aggregation has the benefit of using 
those other classes and all the properties and methods that they contain, without having to keep all those properties and methods in the associated/over-arching class. 

**10. When using composition, when an object is destroyed, what happens to all the objects it is composed of?**

* They are also destroyed. 

**11. When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?**

* They can carry on independently. 
