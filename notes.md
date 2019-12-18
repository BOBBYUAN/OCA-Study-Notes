interface method could be either static or default

interface method if it's static it must be implemented

lamda function predicate , test 

NumberFormat and illegal and checked programmer, rest of them JVM

static initialize can only have static things in it.

package, be careful java doesn't which to use.


Tomorrow need to know：

-- enhanced loop

-- still lamba function

-- compound operator method, the left size must be already declared

-- Date immutable????? or not

-- only inherientace one class (including abstract class), but multiple interfaces

-- string literals are automatically instaniated into a string object

-- watch out the main method name !!!

-- default; break; switch

-- casting, inheritence

-- string indexof return -1 

-- checkout the line!!! missing import

-- casting object doesn not add in memory

-- how many class generate how many bytecode

-- main has a function that include check exception, main has to handle or delcare , o.w. it doesn not compile.

-- All array types are reference
 variables

-- braces not required for for loop and if statement

-- Uppercase sort before lower case

-- can have same method 

-- java8 date and time are in the java.time package

-- do while loop braces watch out

-- concrete class implememnt interface necessary need to add public or no?????

-- lambda function again!!!!!!


========================================================================
non-static initialization block excutes only when instance creates

unreachable statment, compile error

octual literal

we can not access instance variable by class name, but we can access static variable through both

floating point doesn't throw ArithmeticExcetion when dividing by zero

overload method must change the argument list

default even extend, it still only access in the same package

array is passing by reference.

str - the characters to be appended.
offset - the index of the first char to append.
len - the number of chars to append.

sb.setLength -> set array size

indexOf(Charsquence str, int fromIndex)

there is negativeIndex exception

/**   / ingore the effect

even the array is final, the elements of the array are not final

In floating point operation/comparisons, if one argument is floating/double then other one being int is also promoted to the same.

switch statement is more efficient than a set of if-then-else statement

private method cannot be overriden

SuperClass s = new SubClass() // Super class decide what methods could be called, if superclass has the same, the version is in the subClass. static method would go for the reference side

If the supertype version declarea checked exception but the overriding subtype method does not, the compiler thinks you are calling a method that declares an exception.

overriden may not throw bordar or new checked exception, but it's legal to throw bordar or new unchecked exception

((Student)stu).read

as long as its a non-fraction ends with l, it's a valid long literal.

for octual literal, we can only use 0-7 digits

the class object unreachable, the objects in that class would also be unreachable

equals method of the wrapper will first check if the wrapper is the same type

abstract is not valid for variable

in the interface, it could have final variable

%06d filling leading zero with 0

final variable has to be initializedi in three ways

we can't use private access modifier inside the local scope

case constant has to be compile time constant

interface is 100% abstract, but it's not required

downcasting should be explictly

classcasting is not possible for up casting

variables declared inside a method are called local variable

static initilxiation run once when the calss is frist loaded, but instance intixalization run everytime

overloading, we must change the argument list 

static content can't access instance content

static {} could only have static things

stringbuilder doesn't have CharArray

java SE8 introduced new method join

string -> length()

java SE8 introduced splierator for ArrayList

defauly capacity of Arraylist is 10

correctly used (a instanceof C)

try to cast a super class reference to lower class reference, but super class reference refers to super class object, so casting would have classcastingException

A protected member (k) is accessible within all classes in the same package and within subclasses in other packages.

static content can never use (this) since static content deosn't belong to any instance 

Stringbuilder sb = new Stringbuilder(10) -> capacity: 10
Stringbuilder sb = new stringbuilder("ABCD") -> capacity: 16(initial) + 4

A functional interface contains only one or more abstract methods

getMonth -> return March

publci void getChars(int srcBegin, int secEnd, char[] dst, int dstBegin)

public StringBuilder insert(int offset, long l)

e2.join(e1)

every class must have a constructor

wrapper object, nullpointerexception

none of wrapper would wide from one to another

interface vairables ar public, static and final

if statement, might not initialized, so it would cause compile error

Boolean.valueof(true)

overload determined by the number and type of the argument, not return and access modifier

list.set(3,"3"), which is removed.

lambda function variable, used before cause compile error

|| is a short circuit, no need to evaluate expression on the right

String s1 = new String("Java")  creates two objects

ArrayList<Animal> is not super type of ArrayList<Dog>

days.clear() removes all the elements

P1000M

boolean.valueOf, ignore the case

DateTimeException

main method could be overloaded

StringIndexOutoFBoundsException

if there is a statement can't reach, then it would give compile error

unary operator, ++, !, +, --

static method not override

we cannot override private method

assign array different type, compile error not exception

string join, - , A-B-C

switch doesn't allow long, float, double, boolean