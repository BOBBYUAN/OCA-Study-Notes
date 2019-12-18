simulator Entuware java OCA

--String is immutable 
// s.append(3) would not add to s and would be ignored
// however s= s + " two" would add on to string s
1.  += 2 expands to a = a + 2. A String concatenated with any other type gives a String. 
2. We can't store int variable in string variable
3. System.out.println(numbers.substring(7)) // If only one number in the substring, it would go to the end.


--string length v.s. index at 

--substring end-1 position

StringBuilder:
1. append method, mutability 
2. insert and delete before the end position
3. java doesn't allow compare java to stringbuilder
4.  you cannot assign a String to a StringBuilder; instead: StringBuilder b = new StringBuilder("rumble") 

Arrays:
1. binary search negate and then subtract (has to be sorted)
   if not sorted, still compiles fine but would return undefined result.
2. Arrays define a property called length. It is not a method, so parentheses are not allowed. (different than string: length())
3. MultiArray: it is legal to leave out the size for later dimensions of a multidimensional array, the first one is required.

ArrayList:
1. ArrayList and Array both ordered, but Arraylist is NOT fixed size, but array has a fixed size.
2. The ArrayList class defines a method called size().
3. Converting from an array to an ArrayList uses Arrays.asList(names). There is no asList() method on an array instance

Dates and Times:
1. LocalDate does not have a public constructor.
2. A LocalDate does not have a time element, so it can't ad hours.
3. Dates are immutable, so date.plusDays(2) date.plusYears(3) would be ignored.
Period:
1. period.of(1,2,3)
2. Period does not allow chaining. Only the last Period method called counts

Formatting Dates and Times:
1. DateTimeFormatter.ofLocalizedTime(FormatStyle.SHORT) , only outputs the time