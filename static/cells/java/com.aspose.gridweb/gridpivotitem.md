##GridPivotItem
Represents a item in a PivotField report.
**Inheritance:**
java.lang.Object
```
public class GridPivotItem
```
Represents a item in a PivotField report.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDateTimeValue()](#getDateTimeValue--) | Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue |
| [getDoubleValue()](#getDoubleValue--) | Gets the double value of the pivot item If the value is null or not number ,it will return 0 |
| [getIndex()](#getIndex--) | Gets the index of the pivot item in the pivot field |
| [getName()](#getName--) | Gets the name of the pivot item. |
| [getStringValue()](#getStringValue--) | Gets the string value of the pivot item If the value is null, it will return "" |
| [getValue()](#getValue--) | Gets the value of the pivot item |
| [hashCode()](#hashCode--) |  |
| [isHidden()](#isHidden--) | Gets whether the pivot item is hidden. |
| [move(int count)](#move-int-) | Moves the item up or down. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHidden(boolean value)](#setHidden-boolean-) | Sets whether the pivot item is hidden. |
| [setIndex(int value)](#setIndex-int-) | Gets the index of the pivot item in the pivot field |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```
Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue
**Returns:**
[DateTime](../../com.aspose.gridweb/datetime)
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```
Gets the double value of the pivot item If the value is null or not number ,it will return 0
**Returns:**
double
### getIndex() {#getIndex--}
```
public int getIndex()
```
Gets the index of the pivot item in the pivot field
**Returns:**
int
### getName() {#getName--}
```
public String getName()
```
Gets the name of the pivot item.
**Returns:**
java.lang.String
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```
Gets the string value of the pivot item If the value is null, it will return ""
**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```
Gets the value of the pivot item
**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isHidden() {#isHidden--}
```
public boolean isHidden()
```
Gets whether the pivot item is hidden.
**Returns:**
boolean
### move(int count) {#move-int-}
```
public void move(int count)
```
Moves the item up or down.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| count | int | The number of moving up or down. Move the item up if this is less than zero; Move the item down if this is greater than zero. |
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```
Sets whether the pivot item is hidden.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setIndex(int value) {#setIndex-int-}
```
public void setIndex(int value)
```
Gets the index of the pivot item in the pivot field
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### toString() {#toString--}
```
public String toString()
```
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
