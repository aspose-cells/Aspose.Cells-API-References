---
title: RowCollection
second_title: Aspose.Cells for Java API Reference
description: Collects the  objects that represent the individual rows in a worksheet.
type: docs
url: /java/com.aspose.cells/rowcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RowCollection implements Iterable
```

Collects the [Row](../../com.aspose.cells/row) objects that represent the individual rows in a worksheet.

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
```
## Methods

| Method | Description |
| --- | --- |
| [clear()](#clear--) | Clear all rows and cells. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowIndex)](#get-int-) | Gets a [Row](../../com.aspose.cells/row) object by given row index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of rows in this collection. |
| [getRowByIndex(int index)](#getRowByIndex-int-) | Gets the row object by the position in the list. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Gets an enumerator that iterates through this collection |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Remove the row at the specified index |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```


Clear all rows and cells.

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
### get(int rowIndex) {#get-int-}
```
public Row get(int rowIndex)
```


Gets a [Row](../../com.aspose.cells/row) object by given row index. The Row object of given row index will be instantiated if it does not exist before.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int |  |

**Returns:**
[Row](../../com.aspose.cells/row)
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


Gets the number of rows in this collection.

**Returns:**
int
### getRowByIndex(int index) {#getRowByIndex-int-}
```
public Row getRowByIndex(int index)
```


Gets the row object by the position in the list.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position. |

**Returns:**
[Row](../../com.aspose.cells/row) - The Row object at given position.
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


Gets an enumerator that iterates through this collection

```
Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().iterator();
         	while (en.hasNext())
         	{
         	    Row row = (Row)en.next();
         	    System.out.println(row.getIndex() + ": " + row.getHeight());
         	}
```

**Returns:**
java.util.Iterator - enumerator
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


Remove the row at the specified index

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | zero-based row index |

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

