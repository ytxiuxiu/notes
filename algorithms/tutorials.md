# Tutorial 2
1. Write a short program to print out the square numbers Xi = i^2 from i = 0 to a fixed upper limit i = n. All the user has to do is to enter the value for n.

from me
```
INPUT n
REPEAT i FROM 0 TO n
  OUTPUT i^2
```

solution
```
INPUT THE LIMIT N
SET INDEX = 0
WHILE INDEX < 0
  CALCULATE ANS = INDEX * INDEX
  OUTPUT ANS
  INDEX = INDEX + 1
LOOP
```

6. Recursive Fibonnaci numbers with memorization 

```
INPUT x

SET MEMORY TO STORE VALUES

DEFINE FUNCTION fib INPUT n
  IF n = 1 OR n = 2 THEN
    RETURN 1
  ELSE IF n > 2 THEN
    IF n - 2 IS STORED IN THE MEMORY THEN
      SET a = GET VALUE OF n - 2 FROM THE MEMORY
    ELSE
      SET a = CALL FUNCTION fib WITH n = n - 2
    ENDIF
    
    IF n - 1 IS STORED IN THE MEMORY THEN
      SET b = GET VALUE OF n - 1 FROM THE MEMORY
    ELSE
      SET b = CALL FUNCTION fib WITH n = n - 1
    ENDIF
    
    RETURN a + b
    
SET ans = CALL FUNCTION fib WITH n = x
RETURN ans
    