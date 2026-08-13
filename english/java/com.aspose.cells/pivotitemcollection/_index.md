---
title: PivotItemCollection
second_title: Aspose.Cells for Java API Reference
description: Represents all the  objects in the PivotField.
type: docs
url: /java/com.aspose.cells/pivotitemcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotItemCollection extends CollectionBase
```

Represents all the [PivotItem](../../com.aspose.cells/pivotitem) objects in the PivotField.
## Methods

| Method | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [changeitemsOrder(int sourceIndex, int destIndex)](#changeitemsOrder-int-int-) | Directly changes the orders of the two items. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the PivotItem Object at the specific index. |
| [get(String itemValue)](#get-java.lang.String-) | Gets the [PivotItem](../../com.aspose.cells/pivotitem) by the specific name. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [hideAllDetail(boolean isHiddenDetail)](#hideAllDetail-boolean-) | Sets whether to hide all detail of all PivotItems in a pivot field. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Removes the item at the specified index. |
| [swapItem(int index1, int index2)](#swapItem-int-int-) | Directly swap two items. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Adds an item to the CollectionBase instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | The Object to add to the CollectionBase instance. |

**Returns:**
int - The position into which the new element was inserted.
### changeitemsOrder(int sourceIndex, int destIndex) {#changeitemsOrder-int-int-}
```
public void changeitemsOrder(int sourceIndex, int destIndex)
```


Directly changes the orders of the two items.

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotItemCollection.SwapItem() method. This method will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | int | The current index |
| destIndex | int | The dest index |

### clear() {#clear--}
```
public void clear()
```


Removes all objects from the CollectionBase instance.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Return whether instance contains this object

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | test object |

**Returns:**
boolean - Whether instance contains this object
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
public PivotItem get(int index)
```


Gets the PivotItem Object at the specific index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
[PivotItem](../../com.aspose.cells/pivotitem)
### get(String itemValue) {#get-java.lang.String-}
```
public PivotItem get(String itemValue)
```


Gets the [PivotItem](../../com.aspose.cells/pivotitem) by the specific name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| itemValue | java.lang.String |  |

**Returns:**
[PivotItem](../../com.aspose.cells/pivotitem)
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


Gets the number of elements contained in the CollectionBase instance.

**Returns:**
int - The number of elements contained in the CollectionBase instance.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideAllDetail(boolean isHiddenDetail) {#hideAllDetail-boolean-}
```
public void hideAllDetail(boolean isHiddenDetail)
```


Sets whether to hide all detail of all PivotItems in a pivot field. That is collapse/expand this field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isHiddenDetail | boolean | Whether hide the detail of the pivot field. |

### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Determines the index of a specific item in the CollectionBase instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Determines the index of a specific item in the CollectionBase instance. |

**Returns:**
int - The index of value if found in the list; otherwise, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returns an enumerator that iterates through the CollectionBase instance.

**Returns:**
java.util.Iterator - An iterator for the CollectionBase instance.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Removes the item at the specified index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero-based index of the item to remove. |

### swapItem(int index1, int index2) {#swapItem-int-int-}
```
public void swapItem(int index1, int index2)
```


Directly swap two items.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index1 | int |  |
| index2 | int |  |

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

