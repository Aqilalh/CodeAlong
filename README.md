# Notes
SINGLETON-
Singleton is a creational design pattern that lets you ensure that a class has only one instance, while providing a global access point to this instance.
All implementations of the Singleton have these two steps in common:
Make the default constructor private, to prevent other objects from using the new operator with the Singleton class.
Create a static creation method that acts as a constructor. Under the hood, this method calls the private constructor to create an object and saves it in a static field. All following calls to this method return the cached object.

BUILDER-
Builder is a creational design pattern that lets you construct complex objects step by step. The pattern allows you to produce different types and representations of an object using the same construction code.
A Builder class builds the final object step by step. This builder is independent of other objects.
Using builder you can reuse the same object construction code when building different types of products, such as cars, and create the corresponding manuals for them.

Prototype-
Prototype is a creational design pattern that lets you copy existing objects without making your code dependent on their classes.
An object that supports cloning is called a prototype. When your objects have dozens of fields and hundreds of possible configurations, cloning them might serve as an alternative to subclassing.
You can clone objects without coupling to their concrete classes.
You can get rid of repeated initialization code in favor of cloning pre-built prototypes.

Factory-
Factory Method is a creational design pattern that provides an interface for creating objects in a superclass, but allows subclasses to alter the type of objects that will be created.
Use the Factory Method when you don’t know beforehand the exact types and dependencies of the objects your code should work with.
The Factory Method separates product construction code from the code that actually uses the product. Therefore it’s easier to extend the product construction code independently from the rest of the code.
You can introduce new types of products into the program without breaking existing client code.

Abstract-
Abstract Factory is a creational design pattern that lets you produce families of related objects without specifying their concrete classes.
Use the Abstract Factory when your code needs to work with various families of related products, but you don’t want it to depend on the concrete classes of those products—they might be unknown beforehand or you simply want to allow for future extensibility.
You can be sure that the products you’re getting from a factory are compatible with each other.
 You avoid tight coupling between concrete products and client code.
 
 Adapter-
 An Adapter also known as a wrapper class is a structural design pattern that allows objects with incompatible interfaces to collaborate.​
Its main job is to make sure incompatible classes work together.
A class adapter uses inheritance and would only wrap a class.
While an object adapter uses composition and can wrap classes or interfaces.
Use the Adapter class when you want to use some existing class, but its interface isn’t compatible with the rest of your code.
You can introduce new types of adapters into the program without breaking the existing client code, as long as they work with the adapters through the client interface.

Composite-
Composite is a structural design pattern that lets you compose objects into tree structures and then work with these structures as if they were individual objects.
The Composite pattern provides you with two basic element types that share a common interface: simple leaves and complex containers. A container can be composed of both leaves and other containers. This lets you construct a nested recursive object structure that resembles a tree.
 You can work with complex tree structures more conveniently: use polymorphism and recursion to your advantage.
 
Decorator-
Decorator is a structural design pattern that lets you attach new behaviors to objects by placing these objects inside special wrapper objects that contain the behaviors.
Use the Decorator pattern when you need to be able to assign extra behaviors to objects at runtime without breaking the code that uses these objects.
Many programming languages have the final keyword that can be used to prevent further extension of a class. For a final class, the only way to reuse the existing behavior would be to wrap the class with your own wrapper, using the Decorator pattern.
You can extend an object’s behavior without making a new subclass.
You can add or remove responsibilities from an object at runtime.
You can combine several behaviors by wrapping an object into multiple decorators.

Facade-
Facade is a structural design pattern that provides a simplified interface to a library, a framework, or any other complex set of classes.
 Use the Facade pattern when you need to have a limited but straightforward interface to a complex subsystem.
 Create facades to define entry points to each level of a subsystem. You can reduce coupling between multiple subsystems by requiring them to communicate only through facades.
  You can isolate your code from the complexity of a subsystem.
  Facade defines a new interface for existing objects, whereas Adapter tries to make the existing interface usable. Adapter usually wraps just one object, while Facade works with an entire subsystem of objects.
  
  Proxy-
  Proxy is a structural design pattern that lets you provide a substitute or placeholder for another object. A proxy controls access to the original object, allowing you to perform something either before or after the request gets through to the original object.
Instead of creating the object when the app launches, you can delay the object’s initialization to a time when it’s really needed.
 You can control the service object without clients knowing about it.
 You can manage the lifecycle of the service object when clients don’t care about it.
 The proxy works even if the service object isn’t ready or is not available.






