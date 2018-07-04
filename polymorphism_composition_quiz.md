# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

many forms



2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

Where an object can be said to be of more than one type.
E.g A room in a hotel might be of type 'bedroom' as well as of type 'chargeable'



3. What can we use to implement polymorphism in Java?

inheritance - a class inheriting an abstract class and implementing one or more interfaces would have more than one type , or could be said to that it 'IS A' of whatever type the interfaces or abstract class are.

4. How many 'forms' can an object take when using polymorphism?

this would be the number of the interfaces/abstract class it inherited type from, it 'can' take any number.

5. Give an example of when you could use polymorphism.
Bear can ieat a deer, Ieat  honey, don't want a method for 'eatHoney' and 'eatDeer' , saves this to a signle Ieat.eat() method for iEat honey, iEat deer;

modelling an animal say, a deer. Which inherits from a
class "woodland animal" but implements an interface "herbivore"
we might require both types to be used in our model



# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?
(composing an object out of other objects)

A class has an instance or instances of other small class(es), as an attribute or attributes, which allows it to 'inherit' a specific desired behaviour rather than inherit a larger class with specific rigid behaviour to adhere to

7. When would you use composition? Provide a simple example in Java.
When we don't appear to have a clear and single hierarchy. Where we wish to have certain functional behaviours on a subset of the objects, without requiring them to inherit a class full of other functions we don't want to worry about, without the class itself being responsible for the functional behaviour (that is dealt with by the behaviour/ IClass/hasABLE)


8. What is/are the advantage(s) of using composition?

split responsibility into smaller pieces,
Compared to inheritance, smaller 'chunks' of behaviour can be set as objects composition, these behaviours can be switched in and out as required by the needs the user

9. What happens to the behaviours when the object composed of them is destroyed?


the behaviours (which are other objects) are destroyed along with the object whose composition included them.
is this a problem? ;

e.g. car with class engine incrementing mileage, - if car destroyed next car has new engine - 0 mileage.
