Access modifiers:
1. public: method can be called from any class
2. private: method only can be called within the same class
3. protected: method can only be called from classes in the same package or subclasses
4. default: method can only be called from classes in the same package. 

Optional specifiers:
1. static
2. abstract
3. final
4. synchronized (OCP)

Return type: 
Mehthod name: some name avoid

Varargs:
1. must be last element in the parameter
2. walk(1,2,3) // 2

Applying access modifiers:
1. members in the same class (private, defeault, protected, public)
2. member in another class in same package (defauly, protected, public)
3. member in different package but in superclass (protected, public)
4. member in total different package and not superclass (public)

Static method and field:
static variable shared by this class, whatever the class
instance method and variable could use static
but static can not call instance variable and method

Static variable
1. change as program runs
2. another not change, static final = constant (not assign new values)
   BUT, if reference (values.add("changed")) doesn compile

Static initialization:
1. could be initalizated exactly once, and it can not be forgotten

Static import:
1. Static import only for static member not the class
2. order has to be import static

Overloading:
1. varargs same as array, can not overload with the same 

Autoboxing:
1. java would use the most specific version

Constructor:
1 .using this inside the constructor, must be the frist line

Order of initiazialtion:  (block)  static {}  , {}
1. super
2. static
3. instance
4. constructor

if in the same class, static before main

Encapsulating Data:
1. setter and getter

Lambda function:
a -> a.canHop()
(Animal a) -> {return a.canHop();}




