Exam2:

boolean passing string: java boolean value Boolean b1 = new Boolean("tRuE"); // "true" no problem

double and Double different, double primitive type, Double reference type, double coule be auto-boxing to Double

boolean passing string: new Boolean("ture") is "false"

if statement could be only one statement without bracket, after that still need it

switch statement, if not match and no break, keep down, if it already at the lowest position, then can not go down anymore, break.

postfix > prefix
== > && ||
&& > ||
|| is a short-circuit operator, hence no need to evaluate expression on the right

java array can't specifize size when initialize data in it.

same as if statement, while loop only allow on line belongs to him, other than that, still need bracket.

watchout i and arr[i]

int can convert to double, but Integer can not convert to Double,
Integer can convert to int, then int to double

A constuctor should have super() or this(), but can not have both

manually throw an exception --> throw

if throw an exception, but not catch handle would cause compiler error

LocalDate.parse(CharSequence) method accepts String in "9999-99-99" format only, otherwise an exception

date.minusYears(-5) no error, if passing negative, it would add on it.

students.remove(new Student("James", 25)), even remove it would create object in the memory.

list.remove(Object) method returns boolean result but list.remove(int index) returns the removed item from the list

