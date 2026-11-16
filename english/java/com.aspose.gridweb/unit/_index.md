---
title: Unit
second_title: Aspose.Cells for Java API Reference
description: Represents a length measurement
type: docs
url: /java/com.aspose.gridweb/unit/
---

**Inheritance:**
java.lang.Object
```
public class Unit
```

Represents a length measurement
## Constructors

| Constructor | Description |
| --- | --- |
| [Unit()](#Unit--) | the default constructor |
| [Unit(double value, int type)](#Unit-double-int-) | Initializes a new instance of the Unit structure with the specified double precision floating point number and UnitType. |
| [Unit(double value)](#Unit-double-) | Initializes a new instance of the Unit structure with the specified double precision floating point number. |
| [Unit(int value)](#Unit-int-) | Initializes a new instance of the Unit structure with the specified 32-bit signed integer. |
| [Unit(String value)](#Unit-java.lang.String-) | Initializes a new instance of the Unit structure with the specified length. |
## Methods

| Method | Description |
| --- | --- |
| [GetExtension(int type)](#GetExtension-int-) | get string by the type,may get "px" "pt" "%" and so one; |
| [Parse(String s)](#Parse-java.lang.String-) | Converts the specified string to a Unit. |
| [Percentage(double n)](#Percentage-double-) | Creates a Unit of type Percentage from the specified double-precision floating-point number. |
| [Pixel(int n)](#Pixel-int-) | Creates a Unit of type Pixel from the specified 32-bit signed integer. |
| [Point(int n)](#Point-int-) | Creates a Unit of type Point from the specified 32-bit signed integer. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Gets the unit type of the Unit. |
| [getValue()](#getValue--) | Gets the length of the Unit. |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) | Gets a value indicating whether the Unit is empty. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | get string representation of the unit. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Unit() {#Unit--}
```
public Unit()
```


the default constructor

### Unit(double value, int type) {#Unit-double-int-}
```
public Unit(double value, int type)
```


Initializes a new instance of the Unit structure with the specified double precision floating point number and UnitType.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
| type | int |  |

### Unit(double value) {#Unit-double-}
```
public Unit(double value)
```


Initializes a new instance of the Unit structure with the specified double precision floating point number.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### Unit(int value) {#Unit-int-}
```
public Unit(int value)
```


Initializes a new instance of the Unit structure with the specified 32-bit signed integer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### Unit(String value) {#Unit-java.lang.String-}
```
public Unit(String value)
```


Initializes a new instance of the Unit structure with the specified length.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### GetExtension(int type) {#GetExtension-int-}
```
public static String GetExtension(int type)
```


get string by the type,may get "px" "pt" "%" and so one;

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int |  |

**Returns:**
java.lang.String
### Parse(String s) {#Parse-java.lang.String-}
```
public static Unit Parse(String s)
```


Converts the specified string to a Unit.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | java.lang.String |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Percentage(double n) {#Percentage-double-}
```
public static Unit Percentage(double n)
```


Creates a Unit of type Percentage from the specified double-precision floating-point number.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| n | double |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Pixel(int n) {#Pixel-int-}
```
public static Unit Pixel(int n)
```


Creates a Unit of type Pixel from the specified 32-bit signed integer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Point(int n) {#Point-int-}
```
public static Unit Point(int n)
```


Creates a Unit of type Point from the specified 32-bit signed integer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getType() {#getType--}
```
public int getType()
```


Gets the unit type of the Unit.

**Returns:**
int
### getValue() {#getValue--}
```
public double getValue()
```


Gets the length of the Unit.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Gets a value indicating whether the Unit is empty.

**Returns:**
boolean - 
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```


get string representation of the unit.

**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

