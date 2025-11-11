---
title: PivotItem
second_title: Aspose.Cells for Java API Reference
description: Represents a item in a PivotField report.
type: docs
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
| [getFormula()](#getFormula--) | Gets the formula of this calculated item. |
| [getIndex()](#getIndex--) | Gets the index of the pivot item in cache field. |
| [getName()](#getName--) | Gets the name of the pivot item. |
| [getPosition()](#getPosition--) | Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [getPositionInSameParentNode()](#getPositionInSameParentNode--) | Specifying the position index in the PivotItems under the same parent node. |
| [getStringValue()](#getStringValue--) | Gets the string value of the pivot item If the value is null, it will return "" |
| [getValue()](#getValue--) | Gets the value of the pivot item |
| [hashCode()](#hashCode--) |  |
| [hide(boolean value)](#hide-boolean-) | Sets whether the pivot item is hidden. |
| [isCalculatedItem()](#isCalculatedItem--) | Indicates whether this pivot item is a calculated formula item. |
| [isDetailHidden()](#isDetailHidden--) | Gets whether the detail of this pivot item is hidden. |
| [isFormula()](#isFormula--) | Indicates whether this pivot item is a calculated formula item. |
| [isHidden()](#isHidden--) | Gets whether the pivot item is hidden. |
| [isHideDetail()](#isHideDetail--) | Gets whether the pivot item hides detail. |
| [isMissing()](#isMissing--) | Indicates whether the item is removed from the data source. |
| [move(int count, boolean isSameParent)](#move-int-boolean-) | Moves the item up or down |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDetailHidden(boolean value)](#setDetailHidden-boolean-) | Sets whether the detail of this pivot item is hidden. |
| [setFormula(boolean value)](#setFormula-boolean-) | Indicates whether this pivot item is a calculated formula item. |
| [setHidden(boolean value)](#setHidden-boolean-) | Sets whether the pivot item is hidden. |
| [setHideDetail(boolean value)](#setHideDetail-boolean-) | Sets whether the pivot item hides detail. |
| [setIndex(int value)](#setIndex-int-) | Gets the index of the pivot item in cache field. |
| [setName(String value)](#setName-java.lang.String-) | Gets the name of the pivot item. |
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
### getFormula() {#getFormula--}
```
public String getFormula()
```


Gets the formula of this calculated item. Only works when this item is calculated item.

**Returns:**
java.lang.String - 
### getIndex() {#getIndex--}
```
public int getIndex()
```


Gets the index of the pivot item in cache field.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Gets the name of the pivot item.

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


Specifying the position index in all the PivotItems,not the PivotItems under the same parent node.

**Returns:**
int
### getPositionInSameParentNode() {#getPositionInSameParentNode--}
```
public int getPositionInSameParentNode()
```


Specifying the position index in the PivotItems under the same parent node.

**Returns:**
int
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


Sets whether the pivot item is hidden.

**Remarks**

NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Pivot.PivotField.HideItem method. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### isCalculatedItem() {#isCalculatedItem--}
```
public boolean isCalculatedItem()
```


Indicates whether this pivot item is a calculated formula item.

**Returns:**
boolean
### isDetailHidden() {#isDetailHidden--}
```
public boolean isDetailHidden()
```


Gets whether the detail of this pivot item is hidden.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Indicates whether this pivot item is a calculated formula item.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotItem.IsCalculatedItem property instead. This property will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Gets whether the pivot item is hidden.

**Returns:**
boolean
### isHideDetail() {#isHideDetail--}
```
public boolean isHideDetail()
```


Gets whether the pivot item hides detail.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotItem.IsDetailHidden property instead. This property will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isMissing() {#isMissing--}
```
public boolean isMissing()
```


Indicates whether the item is removed from the data source.

**Remarks**

True means this value has been removed from the data source.

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




### setDetailHidden(boolean value) {#setDetailHidden-boolean-}
```
public void setDetailHidden(boolean value)
```


Sets whether the detail of this pivot item is hidden.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFormula(boolean value) {#setFormula-boolean-}
```
public void setFormula(boolean value)
```


Indicates whether this pivot item is a calculated formula item.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotItem.IsCalculatedItem property instead. This property will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Sets whether the pivot item is hidden.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHideDetail(boolean value) {#setHideDetail-boolean-}
```
public void setHideDetail(boolean value)
```


Sets whether the pivot item hides detail.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotItem.IsDetailHidden property instead. This property will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIndex(int value) {#setIndex-int-}
```
public void setIndex(int value)
```


Gets the index of the pivot item in cache field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Gets the name of the pivot item.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

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

