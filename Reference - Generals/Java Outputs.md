## `NaN`: Not a number
- $$ \sqrt(-1) $$
- or division with zero (float only):
$$
\frac{0.0}{0.0} \ or \ \frac{0}{0.0}
$$


## `ArithmeticException`: **Important!**
-  Division any number with zero (integers):
- $$ \frac{3}{0} $$

## `Infinity` or `-Infinity`:
-  Division any number with zero (floats):
$$
\frac{3.0}{0.0} \ or \ \frac{-3.0}{0.0}
$$


## `NullPointerExcpetion`:
- Trying to invoke object with `null` reference:
```java
BankAccount b; //No constructor called.

b.withdraw(acctPassword, amt);
// NullPointerException
```


## `ClassCastException`:
- Run-time Error:
```java
Student u = new UnderGrad();
System.out.println((String) u); //Wrong!
int x = ((GradStudent) u).getID; //Wrong relationship!
```

## `ArrayIndexOutOfBoundsException`:
- Access index `k>=length()` or negative value.

## `StringIndexOutOfBoundsException` :
- substring length exceed length of string or negative.