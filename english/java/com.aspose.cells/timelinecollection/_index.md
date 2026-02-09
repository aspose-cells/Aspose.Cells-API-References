---
title: TimelineCollection
second_title: Aspose.Cells for Java API Reference
description: Specifies the collection of all the  objects on the worksheet.
type: docs
url: /java/com.aspose.cells/timelinecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TimelineCollection extends CollectionBase
```

Specifies the collection of all the [Timeline](../../com.aspose.cells/timeline) objects on the worksheet. It was supported since Excel 2013.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         int pivotIndex = pivots.add("=Sheet1!A1:C5", "A12", "TestPivotTable");
         PivotTable pivot = pivots.get(pivotIndex);
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Refresh PivotTable data
         pivot.refreshData();
         pivot.calculateData();
 
         //do your business
         book.save("out.xlsx");
```
## Methods

| Method | Description |
| --- | --- |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | Add a new Timeline using PivotTable as data source |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | Add a new Timeline using PivotTable as data source |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Add a new Timeline using PivotTable as data source |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | Add a new Timeline using PivotTable as data source |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | Add a new Timeline using PivotTable as data source |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Add a new Timeline using PivotTable as data source |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the Timeline by index. |
| [get(String name)](#get-java.lang.String-) | Gets the Timeline by Timeline's name. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Removes the item at the specified index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


Add a new Timeline using PivotTable as data source

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 20, 5, pivot.getBaseFields().get(1));
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Timeline range. |
| column | int | Column index of the cell in the upper-left corner of the Timeline range. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | The PivotField in PivotTable.BaseFields |

**Returns:**
int - The new add Timeline index
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


Add a new Timeline using PivotTable as data source

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 15, 5, 1);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Timeline range. |
| column | int | Column index of the cell in the upper-left corner of the Timeline range. |
| baseFieldIndex | int | The index of PivotField in PivotTable.BaseFields |

**Returns:**
int - The new add Timeline index
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


Add a new Timeline using PivotTable as data source

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 10, 5, "date");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Timeline range. |
| column | int | Column index of the cell in the upper-left corner of the Timeline range. |
| baseFieldName | java.lang.String | The name of PivotField in PivotTable.BaseFields |

**Returns:**
int - The new add Timeline index
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


Add a new Timeline using PivotTable as data source

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i10", pivot.getBaseFields().get(1));
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| destCellName | java.lang.String | The cell name in the upper-left corner of the Timeline range. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | The PivotField in PivotTable.BaseFields |

**Returns:**
int - The new add Timeline index
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


Add a new Timeline using PivotTable as data source

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i5", 1);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| destCellName | java.lang.String | The cell name in the upper-left corner of the Timeline range. |
| baseFieldIndex | int | The index of PivotField in PivotTable.BaseFields |

**Returns:**
int - The new add Timeline index
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


Add a new Timeline using PivotTable as data source

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i15", "date");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| destCellName | java.lang.String | The cell name in the upper-left corner of the Timeline range. |
| baseFieldName | java.lang.String | The name of PivotField in PivotTable.BaseFields |

**Returns:**
int - The new add Timeline index
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
public Timeline get(int index)
```


Gets the Timeline by index.

**Example**

```
         //Get the Timeline by index.
         Timeline objByIndex = sheet.getTimelines().get(0);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
[Timeline](../../com.aspose.cells/timeline)
### get(String name) {#get-java.lang.String-}
```
public Timeline get(String name)
```


Gets the Timeline by Timeline's name.

**Example**

```
         //Get the Timeline by Timeline's name.
         Timeline objByName = sheet.getTimelines().get("date");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[Timeline](../../com.aspose.cells/timeline)
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Removes the item at the specified index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero-based index of the item to remove. |

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

