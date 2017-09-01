Constructors
---

#### this

```C#
this{value: T}
this{x: T, y: T, z: T}
this{p2d: Point2D<T>, z: T}
```

##### Brief
Creates a new instance initializing each component of the point.

###### param value
the value to use for each component
###### param x
the first dimension of the point
###### param y
the second dimension of the point
###### param z
the third dimension of the point
###### param p2d
a 2 dimensional point that is used as the first two dimensions
***

Methods
---

#### Clamp

```C#
def Clamp(min: Point3D<T>, max: Point3D<T>)
def Clamp(min: T, max: T)
```

##### Brief
Clamps each component of the current mutable instance between `min` and `max`.

###### param min
the minimum value
###### param max
the maximum value
***

#### Clamped

```C#
func Clamped(min: Point3D<T>, max: Point3D<T>)
func Clamped(min: T, max: T)
```

##### Brief
Returns a copy of the color with each component clamped between `min` and `max`.

###### param min
the minimum value
###### param max
the maximum value
###### returns
the clamped value
***

#### GetMin

```C#
func GetMin(min: Point3D<T>)
```

##### Brief
Returns the member-wise minimum between the current instance and the input.

###### param min
the value to test against
###### returns
the member-wise minimum
***

#### GetMax

```C#
func GetMax(max: Point3D<T>)
```

##### Brief
Returns the member-wise maximum between the current instance and the input.

###### param max
the value to test against
###### returns
the member-wise maximum
***

#### IsNormalized

```C#
func IsNormalized(tolerance: T)
```

##### Brief
Tests if the current instance is a 3 dimensional normalized vector, within a tolerance.

###### param tolerance
tolerance for a non zero lengthed vector
###### returns

***

#### Normalize

```C#
def Normalize(tolerance: T)
```

##### Brief
Normalizes the 3 dimensional vector if its length falls within the tolerance limits.

Otherwise, the value remains unchanged.

###### param tolerance
tolerance for a non zero lengthed vector
***

#### Normalized

```C#
func Normalized(tolerance: T)
```

##### Brief
Returns a 3 dimensional normalized copy of the vector if its length falls within the tolerance limits.

Otherwise, returns the value as is.

###### param tolerance
tolerance for a non zero lengthed vector
###### returns

***

#### @add

```C#
func @add(second: Point3D<T>)
func @add(second: T)
```

##### Brief
Member-wise addition operator. Commutative.

###### param second
the second operand
###### returns

***

#### @sub

```C#
static func @sub(left: Point3D<T>, right: Point3D<T>)
static func @sub(left: Point3D<T>, right: T)
static func @sub(left: T, right: Point3D<T>)
```

##### Brief
Member-wise subtraction operator.

###### param left
the left operand
###### param right
the right operand
###### returns

***

#### @mul

```C#
func @mul(second: Point3D<T>)
func @mul(second: T)
```

##### Brief
Member-wise multiplication operator. Commutative.

###### param second
the second operand
###### returns

***

#### @div

```C#
static func @div(left: Point3D<T>, right: Point3D<T>)
static func @div(left: Point3D<T>, right: T)
static func @div(left: T, right: Point3D<T>)
```

##### Brief
Member-wise division operator.

###### param left
the left operand
###### param right
the right operand
###### returns

***

#### @mod

```C#
static func @mod(left: Point3D<T>, right: Point3D<T>)
static func @mod(left: Point3D<T>, right: T)
static func @mod(left: T, right: Point3D<T>)
```

##### Brief
Member-wise modulo operator.

###### param left
the left operand
###### param right
the right operand
###### returns

***

#### @minus

```C#
func @minus()
```

##### Brief
Returns the member-wise negative of the current instance.

###### returns

***

#### @eq

```C#
func @eq(second: T)
```

##### Brief
Member-wise equality operator.

###### param second
the second operand
###### returns

***

#### @neq

```C#
func @neq(second: T)
```

##### Brief
Member-wise inequality operator.

###### param second
the second operand
###### returns

***

#### Equals

```C#
func Equals(second: Point3D<T>, tolerance: T)
func Equals(second: T, tolerance: T)
```

##### Brief
Member-wise equality operator within a given tolerance.

###### param second
the second operand
###### param tolerance
tolerance for equality
###### returns

***

Properties
---

#### Length

```C#
property Length: T; get;
```

##### Brief
The length of the instance interpreted as a 3 dimensional vector.

***

#### LengthSquared

```C#
property LengthSquared: T; get;
```

##### Brief
The squred length of the instance interpreted as a 3 dimensional vector.

***

Variables
---

#### X

```C#
val X: T
```

##### Brief
The first dimension of the point.

***

#### Y

```C#
val Y: T
```

##### Brief
The second dimension of the point.

***

#### Z

```C#
val Z: T
```

##### Brief
The third dimension of the point.

***
