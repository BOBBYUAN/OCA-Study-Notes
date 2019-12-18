Exceptions:
1. checked and unchecked exceptions (RuntimeException)

try statement:
1. On OCA, a try statement must have catch and/or finally.
2. try + {}
3. order: try, then catch, then finally

Catching various exception:
1. subclass need to up, superclass need to down.

Runtime Exceptions:
Checked Exceptions:
Error:

Calling methods that throw exceptions:
declare exception
handle exception

subclass could declare fewer, not add new or more (only for checked exception)

but it's ok for runtime exception

----------------------------------------------------------
Flashcards:
-- try must follow somethings
-- Runtime exception also called uncheck exception
-- declare a exception, [throws], to actually throw exception in the {}. [throw new], 
-- only Illegal and NumberFormat throw by the programmer, the rest of them throw by JVM
-- the catch order is important, sub calss have to before the sup class, ow it would has a compile error.
-- can not allowed bordar in the body, runtime exception could be throw in any methods, and all exception when declare not require to throw in the body
-- 