
## De Morgan's Laws:  
 $$ !(A \ || \ B) = !A \ \&\& \ !B $$
$$ !(A \ \&\& \ B) = !A \ || \ !B $$
## Precedence:
- (1): `!, ++, --`
- (2): `*, /, %`
- (3): `+, -`
- (4): `>, <, <=, >=`
- (5): `==, !=`
- (6): `&&`
- (7): `||`
- (8): `=, +=, -=, *=, /=, %=`
## `equals` method: For both objects and Strings!!
- == means share same memory slot: **ATTENTION: do not use on Strings**
- Equals: same content.
```java
Date d1 = new Date("January", 14, 2001);
Date d2 = d1;
Date d3 = new Date("January", 14, 2001);


d1.equals(d2) == true
d1 == d2: true
d1 == d3: false
```

## String length: `a.length()`
## List length: `l.length`: Attention: NO brackets.
## `ArrayList` length: `al.size()`
## String index: `a.indexOf(String s)`
## Random: `Math.random()`: 0.0 <= r < 1.0
- Random within range: `Math.random() * range + low`

### - When an array is passed as a parameter, it is possible to alter the contents of the array.