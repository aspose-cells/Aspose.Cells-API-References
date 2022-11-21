---
title: PivotItem
second_title: Aspose.Cells for Java API Reference
description: Represents a item in a PivotField report.
type: docs
weight: 407
url: /java/com.aspose.cells/pivotitem/
---

**Inheritance:**
java.lang.Object
```
public class PivotItem
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
| [hide(boolean value)](#hide-boolean-) | Sets whether the pivot item is hidden. |
| [isHidden()](#isHidden--) | Gets and Sets whether the pivot item is hidden. |
| [isHideDetail()](#isHideDetail--) | Gets and Sets whether the pivot item hides detail. |
| [move(int count, boolean isSameParent)](#move-int-boolean-) | Moves the item up or down |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHidden(boolean value)](#setHidden-boolean-) | For the description of this property, please see [isHidden()](../../com.aspose.cells/pivotitem\#isHidden--) |
| [setHideDetail(boolean value)](#setHideDetail-boolean-) | For the description of this property, please see [isHideDetail()](../../com.aspose.cells/pivotitem\#isHideDetail--) |
| [setIndex(int value)](#setIndex-int-) | For the description of this property, please see [getIndex()](../../com.aspose.cells/pivotitem\#getIndex--) |
| [setPosition(int value)](#setPosition-int-) | Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [setPositionInSameParentNode(int value)](#setPositionInSameParentNode-int-) | Specifying the position index in the PivotItems under the same parent node. |
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
[DateTime](../../com.aspose.cells/datetime)
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
### hide(boolean value) {#hide-boolean-}
```
public void hide(boolean value)
```


Sets whether the pivot item is hidden. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Pivot.PivotField.HideItem method. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Gets and Sets whether the pivot item is hidden.

**Returns:**
boolean
### isHideDetail() {#isHideDetail--}
```
public boolean isHideDetail()
```


Gets and Sets whether the pivot item hides detail.

**Returns:**
boolean
### move(int count, boolean isSameParent) {#move-int-boolean-}
```
public void move(int count, boolean isSameParent)
```


Moves the item up or down

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| count | int | The number of moving up or down. Move the item up if this is less than zero; Move the item down if this is greater than zero. |
| isSameParent | boolean | Specifying whether moving operation is in the same parent node or not |

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


For the description of this property, please see [isHidden()](../../com.aspose.cells/pivotitem\#isHidden--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHideDetail(boolean value) {#setHideDetail-boolean-}
```
public void setHideDetail(boolean value)
```


For the description of this property, please see [isHideDetail()](../../com.aspose.cells/pivotitem\#isHideDetail--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIndex(int value) {#setIndex-int-}
```
public void setIndex(int value)
```


For the description of this property, please see [getIndex()](../../com.aspose.cells/pivotitem\#getIndex--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Specifying the position index in all the PivotItems,not the PivotItems under the same parent node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPositionInSameParentNode(int value) {#setPositionInSameParentNode-int-}
```
public void setPositionInSameParentNode(int value)
```


Specifying the position index in the PivotItems under the same parent node.

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

