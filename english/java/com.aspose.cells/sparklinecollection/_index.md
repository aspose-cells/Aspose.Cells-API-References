---
title: SparklineCollection
second_title: Aspose.Cells for Java API Reference
description: Encapsulates a collection of  objects.
type: docs
url: /java/com.aspose.cells/sparklinecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SparklineCollection extends CollectionBase
```

Encapsulates a collection of [Sparkline](../../com.aspose.cells/sparkline) objects.

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
 
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, sheet.getName() + "!A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         book.save("output.xlsx", SaveFormat.XLSX);
```
## Methods

| Method | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [add(String dataRange, int row, int column)](#add-java.lang.String-int-int-) | Add a sparkline. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [Sparkline](../../com.aspose.cells/sparkline) element at the specified index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Object o)](#remove-java.lang.Object-) | Removes the sparkline |
| [removeAt(int index)](#removeAt-int-) | Removes the item at the specified index. |
| [removeSparkline(Sparkline o)](#removeSparkline-com.aspose.cells.Sparkline-) | Removes the sparkline |
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
### add(String dataRange, int row, int column) {#add-java.lang.String-int-int-}
```
public int add(String dataRange, int row, int column)
```


Add a sparkline.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | java.lang.String | Specifies the new data range of the sparkline. |
| row | int | The row index of the location. |
| column | int | The column index of the location. |

**Returns:**
int
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
public Sparkline get(int index)
```


Gets the [Sparkline](../../com.aspose.cells/sparkline) element at the specified index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |

**Returns:**
[Sparkline](../../com.aspose.cells/sparkline) - The element at the specified index.
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




### remove(Object o) {#remove-java.lang.Object-}
```
public void remove(Object o)
```


Removes the sparkline

**Remarks**

NOTE: This member is now obsolete. Instead, please use RemoveSparkline() method. This method will be removed 6 months later since December 2025. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Removes the item at the specified index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero-based index of the item to remove. |

### removeSparkline(Sparkline o) {#removeSparkline-com.aspose.cells.Sparkline-}
```
public void removeSparkline(Sparkline o)
```


Removes the sparkline

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | [Sparkline](../../com.aspose.cells/sparkline) |  |

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

