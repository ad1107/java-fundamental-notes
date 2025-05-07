- `int` can be casted **and will always find a way** to a `double`. 

- But `double` cant be turned into int. Needs a cast
```JAVA
int num = 5;
double realnum = num;

double realnum2 = 6.89;
int num2 = (int) realnum2; //Cast!
```
- `int` division to get double
``` java
 int total, n;
 double average = (double) total / n;


// INCORRECT:
double average = (double) (total / n);
// This part will turn into int before into a double
```

- Remember these outputs:
![[Java Outputs#`Infinity` or `-Infinity`]]

![[Java Outputs#`ArithmeticException` **Important!**]]

![[Java Outputs#`NaN` Not a number]]




- **AVOID: Comparing double numbers!!!** - Not tested.

- `final`: constant: Assign once, assign more will fail.

![[Java Syntax#De Morgan's Laws]]

![[Java Syntax#Precedence]]
