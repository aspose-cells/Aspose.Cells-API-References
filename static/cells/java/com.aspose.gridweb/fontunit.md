##FontUnit
Represents the size of a font.
**Inheritance:**
java.lang.Object
```
public class FontUnit
```
Represents the size of a font.
## Constructors
| Constructor | Description |
| --- | --- |
| [FontUnit()](#FontUnit--) | The default constructor . |
| [FontUnit(int value)](#FontUnit-int-) | Initializes a new instance of the FontUnit class with the specified font size. |
| [FontUnit(double value)](#FontUnit-double-) | Initializes a new instance of the FontUnit class with the specified font size in points. |
| [FontUnit(double value, int type)](#FontUnit-double-int-) | Initializes a new instance of the FontUnit class with the specified font size and UnitType value. |
| [FontUnit(Unit value)](#FontUnit-com.aspose.gridweb.Unit-) | Initializes a new instance of the FontUnit class with the specified Unit. |
| [FontUnit(String value)](#FontUnit-java.lang.String-) | Initializes a new instance of the FontUnit class with the specified string. |
## Fields
| Field | Description |
| --- | --- |
| [Empty](#Empty) | Specifies an empty FontUnit. |
| [Large](#Large) | Specifies a FontUnit with LARGE font. |
| [Larger](#Larger) | Specifies a FontUnit with Larger font. |
| [Medium](#Medium) | Specifies a FontUnit with MEDIUM font. |
| [Small](#Small) | Specifies a FontUnit with SMALL font. |
| [Smaller](#Smaller) | Specifies a FontUnit with Smaller font. |
| [XLarge](#XLarge) | Specifies a FontUnit with X\_LARGE font. |
| [XSmall](#XSmall) | Specifies a FontUnit with X\_SMALL font. |
| [XXLarge](#XXLarge) | Specifies a FontUnit with XX\_LARGE font. |
| [XXSmall](#XXSmall) | Specifies a FontUnit with XX\_SMALL font. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | returns the font size type. |
| [getUnit()](#getUnit--) | Gets a Unit that represents the font size. |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) | check whether the font size is empty or not. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parse(String s)](#parse-java.lang.String-) | Converts the specified string to its FontUnit equivalent. |
| [point(int n)](#point-int-) | Creates a FontUnit of type Point from an integer value. |
| [toString()](#toString--) | Converts the FontUnit object to a string representation. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FontUnit() {#FontUnit--}
```
public FontUnit()
```
The default constructor .
### FontUnit(int value) {#FontUnit-int-}
```
public FontUnit(int value)
```
Initializes a new instance of the FontUnit class with the specified font size.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### FontUnit(double value) {#FontUnit-double-}
```
public FontUnit(double value)
```
Initializes a new instance of the FontUnit class with the specified font size in points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### FontUnit(double value, int type) {#FontUnit-double-int-}
```
public FontUnit(double value, int type)
```
Initializes a new instance of the FontUnit class with the specified font size and UnitType value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
| type | int |  |
### FontUnit(Unit value) {#FontUnit-com.aspose.gridweb.Unit-}
```
public FontUnit(Unit value)
```
Initializes a new instance of the FontUnit class with the specified Unit.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |
### FontUnit(String value) {#FontUnit-java.lang.String-}
```
public FontUnit(String value)
```
Initializes a new instance of the FontUnit class with the specified string.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### Empty {#Empty}
```
public static FontUnit Empty
```
Specifies an empty FontUnit.
### Large {#Large}
```
public static FontUnit Large
```
Specifies a FontUnit with LARGE font.
### Larger {#Larger}
```
public static FontUnit Larger
```
Specifies a FontUnit with Larger font.
### Medium {#Medium}
```
public static FontUnit Medium
```
Specifies a FontUnit with MEDIUM font.
### Small {#Small}
```
public static FontUnit Small
```
Specifies a FontUnit with SMALL font.
### Smaller {#Smaller}
```
public static FontUnit Smaller
```
Specifies a FontUnit with Smaller font.
### XLarge {#XLarge}
```
public static FontUnit XLarge
```
Specifies a FontUnit with X\_LARGE font.
### XSmall {#XSmall}
```
public static FontUnit XSmall
```
Specifies a FontUnit with X\_SMALL font.
### XXLarge {#XXLarge}
```
public static FontUnit XXLarge
```
Specifies a FontUnit with XX\_LARGE font.
### XXSmall {#XXSmall}
```
public static FontUnit XXSmall
```
Specifies a FontUnit with XX\_SMALL font.
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
returns the font size type.
**Returns:**
int -
### getUnit() {#getUnit--}
```
public Unit getUnit()
```
Gets a Unit that represents the font size.
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
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
check whether the font size is empty or not.
**Returns:**
boolean - bool value
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
public static FontUnit parse(String s)
```
Converts the specified string to its FontUnit equivalent.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | java.lang.String |  |
**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### point(int n) {#point-int-}
```
public static FontUnit point(int n)
```
Creates a FontUnit of type Point from an integer value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| n | int |  |
**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### toString() {#toString--}
```
public String toString()
```
Converts the FontUnit object to a string representation.
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
