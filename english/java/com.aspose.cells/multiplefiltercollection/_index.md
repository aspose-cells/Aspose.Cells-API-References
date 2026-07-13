---
title: MultipleFilterCollection
second_title: Aspose.Cells for Java API Reference
description: Represents the multiple filter collection.
type: docs
url: /java/com.aspose.cells/multiplefiltercollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class MultipleFilterCollection implements Iterable
```

Represents the multiple filter collection.

**Remarks**

NOTE: This class is now obsolete. Instead,please use [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) instead. This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.
## Constructors

| Constructor | Description |
| --- | --- |
| [MultipleFilterCollection()](#MultipleFilterCollection--) | Constructs one new instance. |
## Methods

| Method | Description |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | Adds a date filter criteria value. |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | Adds a date time filter criteria value. |
| [add(String filter)](#add-java.lang.String-) | Adds a label filter criteria. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) or a string value. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the count of the filter values. |
| [getMatchBlank()](#getMatchBlank--) | Indicates whether to filter by blank. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Get the enumerator for filter value, |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | Indicates whether to filter by blank. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MultipleFilterCollection() {#MultipleFilterCollection--}
```
public MultipleFilterCollection()
```


Constructs one new instance.

**Remarks**

NOTE: This member is now obsolete. Instead,please set FilterColumn.FilterType as FilterType.MultipleFilters then get FilterColumn.MultipleFilters. This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

### add(int type, int year, int month, int day) {#add-int-int-int-int-}
```
public void add(int type, int year, int month, int day)
```


Adds a date filter criteria value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). The type of date filter. |
| year | int | The year. |
| month | int | The month. |
| day | int | The day. |

### add(int type, int year, int month, int day, int hour, int minute, int second) {#add-int-int-int-int-int-int-int-}
```
public void add(int type, int year, int month, int day, int hour, int minute, int second)
```


Adds a date time filter criteria value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). The type of date filter. |
| year | int | The year. |
| month | int | The month. |
| day | int | The day. |
| hour | int | The hour. |
| minute | int | The minute. |
| second | int | The second. |

### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


Adds a label filter criteria.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filter | java.lang.String | The filter data. |

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
### get(int index) {#get-int-}
```
public Object get(int index)
```


Gets [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) or a string value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
java.lang.Object - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Gets the count of the filter values.

**Returns:**
int
### getMatchBlank() {#getMatchBlank--}
```
public boolean getMatchBlank()
```


Indicates whether to filter by blank.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Get the enumerator for filter value,

**Returns:**
java.util.Iterator - 
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setMatchBlank(boolean value) {#setMatchBlank-boolean-}
```
public void setMatchBlank(boolean value)
```


Indicates whether to filter by blank.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

