---
title: PivotFieldGroupOptions
second_title: Aspose.Cells for Java API Reference
description: Options for pivot field grouping settings.
type: docs
url: /java/com.aspose.cells/pivotfieldgroupoptions/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldGroupOptions
```

Options for pivot field grouping settings.
## Constructors

| Constructor | Description |
| --- | --- |
| [PivotFieldGroupOptions()](#PivotFieldGroupOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndDate()](#getEndDate--) | Gets the end value of the grouping range. |
| [getEndNumber()](#getEndNumber--) | Gets the end value of the grouping range. |
| [getGroupType()](#getGroupType--) | Gets the grouping type for pivot field. |
| [getGroupTypes()](#getGroupTypes--) | Gets the grouping type for pivot field. |
| [getInterval()](#getInterval--) | Gets the interval size for each group. |
| [getNewPivotField()](#getNewPivotField--) | Gets a value indicating whether new pivot fields should be created after grouping. |
| [getStartDate()](#getStartDate--) | Gets the start value of the grouping range. |
| [getStartNumber()](#getStartNumber--) | Gets the start value of the grouping range. |
| [hashCode()](#hashCode--) |  |
| [isAutoEnd()](#isAutoEnd--) | Gets a value indicating whether the end value is automatically determined. |
| [isAutoStart()](#isAutoStart--) | Gets a value indicating whether the start value is automatically determined. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoEnd(boolean value)](#setAutoEnd-boolean-) | Sets a value indicating whether the end value is automatically determined. |
| [setAutoStart(boolean value)](#setAutoStart-boolean-) | Sets a value indicating whether the start value is automatically determined. |
| [setEndDate(DateTime value)](#setEndDate-com.aspose.cells.DateTime-) | Sets the end value of the grouping range. |
| [setEndNumber(double value)](#setEndNumber-double-) | Sets the end value of the grouping range. |
| [setGroupType(int value)](#setGroupType-int-) | Sets the grouping type for pivot field. |
| [setGroupTypes(int[] value)](#setGroupTypes-int---) | Sets the grouping type for pivot field. |
| [setInterval(double value)](#setInterval-double-) | Sets the interval size for each group. |
| [setNewPivotField(boolean value)](#setNewPivotField-boolean-) | Sets a value indicating whether new pivot fields should be created after grouping. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Sets the start value of the grouping range. |
| [setStartNumber(double value)](#setStartNumber-double-) | Sets the start value of the grouping range. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotFieldGroupOptions() {#PivotFieldGroupOptions--}
```
public PivotFieldGroupOptions()
```


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
### getEndDate() {#getEndDate--}
```
public DateTime getEndDate()
```


Gets the end value of the grouping range.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getEndNumber() {#getEndNumber--}
```
public double getEndNumber()
```


Gets the end value of the grouping range.

**Returns:**
double
### getGroupType() {#getGroupType--}
```
public int getGroupType()
```


Gets the grouping type for pivot field. Only for grouping date time pivot field.

See [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Example**

```
         // Group by year and month together
         PivotFieldGroupOptions opts = new PivotFieldGroupOptions();
         opts.setGroupType(PivotGroupByType.YEARS | PivotGroupByType.MONTHS);
```

**Returns:**
int
### getGroupTypes() {#getGroupTypes--}
```
public int[] getGroupTypes()
```


Gets the grouping type for pivot field.

See [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

The order in this property will be ignored. When specifying multiple group types, base group fields will be inserted in ascending order and show group field to row/column region in descending order (Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds).

**Returns:**
int[]
### getInterval() {#getInterval--}
```
public double getInterval()
```


Gets the interval size for each group.

**Remarks**

Only for number and days group.

**Returns:**
double
### getNewPivotField() {#getNewPivotField--}
```
public boolean getNewPivotField()
```


Gets a value indicating whether new pivot fields should be created after grouping.

**Remarks**

If not explicitly set, the default value is false for numeric grouping and true for date-time grouping. Only works for the first new group pivot field of the base field.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Gets the start value of the grouping range.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getStartNumber() {#getStartNumber--}
```
public double getStartNumber()
```


Gets the start value of the grouping range.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoEnd() {#isAutoEnd--}
```
public boolean isAutoEnd()
```


Gets a value indicating whether the end value is automatically determined.

**Remarks**

If [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) or [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) is set, this property will be false.

**Returns:**
boolean
### isAutoStart() {#isAutoStart--}
```
public boolean isAutoStart()
```


Gets a value indicating whether the start value is automatically determined.

**Remarks**

If [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) or [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) is set, this property will be false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoEnd(boolean value) {#setAutoEnd-boolean-}
```
public void setAutoEnd(boolean value)
```


Sets a value indicating whether the end value is automatically determined.

**Remarks**

If [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) or [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) is set, this property will be false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoStart(boolean value) {#setAutoStart-boolean-}
```
public void setAutoStart(boolean value)
```


Sets a value indicating whether the start value is automatically determined.

**Remarks**

If [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) or [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) is set, this property will be false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEndDate(DateTime value) {#setEndDate-com.aspose.cells.DateTime-}
```
public void setEndDate(DateTime value)
```


Sets the end value of the grouping range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setEndNumber(double value) {#setEndNumber-double-}
```
public void setEndNumber(double value)
```


Sets the end value of the grouping range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setGroupType(int value) {#setGroupType-int-}
```
public void setGroupType(int value)
```


Sets the grouping type for pivot field. Only for grouping date time pivot field.

See [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setGroupTypes(int[] value) {#setGroupTypes-int---}
```
public void setGroupTypes(int[] value)
```


Sets the grouping type for pivot field.

See [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

The order in this property will be ignored. When specifying multiple group types, base group fields will be inserted in ascending order and show group field to row/column region in descending order (Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int[] |  |

### setInterval(double value) {#setInterval-double-}
```
public void setInterval(double value)
```


Sets the interval size for each group.

**Remarks**

Only for number and days group.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setNewPivotField(boolean value) {#setNewPivotField-boolean-}
```
public void setNewPivotField(boolean value)
```


Sets a value indicating whether new pivot fields should be created after grouping.

**Remarks**

If not explicitly set, the default value is false for numeric grouping and true for date-time grouping. Only works for the first new group pivot field of the base field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Sets the start value of the grouping range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setStartNumber(double value) {#setStartNumber-double-}
```
public void setStartNumber(double value)
```


Sets the start value of the grouping range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

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

