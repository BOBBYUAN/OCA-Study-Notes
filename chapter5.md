Class design:
1. The first statement of every constructor is either a call to another constructor within the class, using this(), or a call to parents constructor using super()
2. this() and super() only in the first line in the constructor and once.
3. in the class, not necessary to write constructor and super in constructor, java would automaically create default one and convert to last one.
4. but if it doesn't have no argument constuctor, java would not help, we have to write by ourselves when we extends, but in the parent still compiles.
5. in the child class, using super and this to access things in partent class, but if overriden, it would be different

------------------------------------------------------------------------------------------

Overriding methods:
1. The method in the child class must have the same signature as the method in the partent class.
2. The method in the child class must be at least accessable or wider.
3. The method in the child class throw excepetion must NOT be new or bordar.
4. If the method return value, it must be the same or a subclass of the method in the partent class. (covariant return type)
5. Difference between override and overload (overload is that it could change the signature, and the reuturn type could be changed.)
6. private method same name, it could compile if in the child redeclare, now it's a new method (private) in child class and the private method in the parent (private) would be hidden.
7. final methods can not be overriden

Hidding Static Method:
1. The method in the child class must have the same signature as the method in the partent class.
2. The method in the child class must be at least accessable or wider.
3. The method in the child class throw excepetion must NOT be new or bordar.
4. If the method return value, it must be the same or a subclass of the method in the partent class. (covariant return type)
(first four rules same as overriding methods)
5. parent method (static) -> child method(static) || parent method (not static) -> child method(not static)
6. Difference between overriding and hiding methods, hiding methods could still keep the things in parent class(false true), however overriding it would replace in the child class (true true)

Inheriting variables:
1. Java doesn't allow inherit variable, but instear hidden variable. (no code change)


------------------------------------------------------------------------------------------

Abstract class:
1. Abstrac class cannot be instantiated directly
2. Abstract class could have any number abstract methods.
3. Abstract can not be private, protected or final.
4. abstract class can inherit another abstract class all of its abstract methods as tis own
5. The first class extends an extend class must implement all inherieted abstract methods.

Abstract methods:
1. abstract methods only be defined in abstract class
2. abstract methods can not be private or final
3. abstract methods must NOT provide body { } when its declared
4. implement an abstract method in subclass same as overriding a method. name and signatrure must be same and must be wide accessable.

------------------------------------------------------------------------------------------


Interface:  (inheritance using implements)
(1).Interface methods:

    1. Interface can not be instantiated dierctly 
        WalksOnTwoLegs example = new WalksOnTwoLegs();  // doesn't compile
    2. Interface is not required to have methods
    3. Assume to have public or default access. 
    It would automatically convert to public abstract (not default methods)

    Inheriting interface: (interface extends interface)
    1. could havem multiple interface inheritence (extends HasTail, HasWhiskers)
    2. the first class that implement interface or extends an abstract class that inplements an interface, need to implement all the methods.

    -- abstract class could implments interface without giving implementation

    --class could not extends interface
    --interface could not extends class

    --inherits two same interfaces -> duplicates, only need one since they have the same signature.

    --inherits two methods with same name and input paramaters, BUT different reutrn type -> not compile

(2). Interface variables:
    1. interface variable assumed public,static,final, anyother would casue error
    2. since it is final, the value must be set when it is declared


(3). Default interface methods. (if you change interface, thousands of developers have to upload thus)
    1. default method only in interface 
    2. it has keyword default, and it has provide the body { }
    3. still public, but not assumed to be static, final or abstract
    4. could be overriden 
    -- if it's override, keep in mind it need key word default  (interface extends interface)
    -- could be replaced, original default same name -> abstract method same name  (interface extends interface)

    -- inherits two same default method without doesn't work (interface extends interface)
    -- .............with overriden it works

(4) Static interface methods:
    println(getJumpHeight()) // not compile
    println(Hop.getJumpHeight()) //compile


------------------------------------------------------------------------------------------

Polymorphism:
1. the type of the object determines which properties exit within the object in memory. (new Cat())
2. The type of the reference to the object determines which methods and variables are accessible to the java program. (Cat) ---version of which one

Casting Objects:
1. Casting an object from a subclass to a superclass doesn't require an explicit cast. (down -> up)
2. Casting an object from a superclass to a subclass requires an explicit cast.  (up -> down)
3. The compiler will not allow casts to unrelated types.
4. Even when the code compiles without issue, an exception may be thrown at runtime if the object being casat is not actually an instance of that class.

Virtual methods:
two types, releated

Polymorphic parameters:
feed(Reptile reptile) sub ->sup

Polymorphism and method overriding:
same overriding.