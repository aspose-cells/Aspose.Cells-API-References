##Unit
Represents a length measurement
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
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getExtension(int type)](#getExtension-int-) | get string by the type,may get "px" "pt" "%" and so one; |
| [getType()](#getType--) | Gets the unit type of the Unit. |
| [getValue()](#getValue--) | Gets the length of the Unit. |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) | Gets a value indicating whether the Unit is empty. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parse(String s)](#parse-java.lang.String-) | Converts the specified string to a Unit. |
| [percentage(double n)](#percentage-double-) | Creates a Unit of type Percentage from the specified double-precision floating-point number. |
| [pixel(int n)](#pixel-int-) | Creates a Unit of type Pixel from the specified 32-bit signed integer. |
| [point(int n)](#point-int-) | Creates a Unit of type Point from the specified 32-bit signed integer. |
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
### getExtension(int type) {#getExtension-int-}
```
public static String getExtension(int type)
```
get string by the type,may get "px" "pt" "%" and so one;
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int |  |
**Returns:**
java.lang.String
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
### parse(String s) {#parse-java.lang.String-}
```
public static Unit parse(String s)
```
Converts the specified string to a Unit.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | java.lang.String |  |
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### percentage(double n) {#percentage-double-}
```
public static Unit percentage(double n)
```
Creates a Unit of type Percentage from the specified double-precision floating-point number.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| n | double |  |
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### pixel(int n) {#pixel-int-}
```
public static Unit pixel(int n)
```
Creates a Unit of type Pixel from the specified 32-bit signed integer.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| n | int |  |
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### point(int n) {#point-int-}
```
public static Unit point(int n)
```
Creates a Unit of type Point from the specified 32-bit signed integer.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| n | int |  |
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
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
