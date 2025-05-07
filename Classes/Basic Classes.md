## `static`: Provide global access, no need to create new object.
- 
```java
public class Employee {
	private string name;
	private static int employeeCount = 0;

	public static int getEmployeeCount(){
		return employeeCount;
	}


Invocation: int employeeTotal = Employee.getEmployeeCount();
```


## Avoid aliasing memory slots in Reference data types:
```java
Date d = new Date(2, 17, 1948);

Date birthday = d; 
// Wrong! Can cause multiple objects to be altered when doing this:
d.changeDate();

//Instead:
Date birthday = new Date(d.getMonth(), d.getDay(), d.getYear());
```

## `null` reference:
- Uninitialized: Constructor hasn't been called.
```java
BankAccount b;
```
- You can make it `null` by doing:
``` java
b = null;
```
![[Java Outputs#`NullPointerExcpetion`]]


## Warning: Passive Primitive Types as Parameters:

```java
public class ParamTest{
	public static void foo(int x, double y){
		x = 3;
		y = 2.5;
	}
	public static void main(String[] args){
		int a = 7;
		double b = 6.5;
		foo(a, b); //Makes a copy to work for the functions
		System.out.println(a + " " + b); --> 7 6.5
	}
}
```


- Next: [[Inheritance and Polymorphism]]