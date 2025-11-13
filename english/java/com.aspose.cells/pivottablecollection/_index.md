---
title: PivotTableCollection
second_title: Aspose.Cells for Java API Reference
description: Represents the collection of all the PivotTable objects on the specified worksheet.
type: docs
url: /java/com.aspose.cells/pivottablecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableCollection extends CollectionBase
```

Represents the collection of all the PivotTable objects on the specified worksheet.

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
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         int pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable");
         PivotTable pivot = pivots.get(pivotIndex);
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         int index = pivot.getPivotFilters().add(0, PivotFilterType.COUNT);
         PivotFilter filter = pivot.getPivotFilters().get(index);
         filter.getAutoFilter().filterTop10(0, false, false, 2);
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getPivotFormatConditions().add();
         PivotFormatCondition pfc = pivot.getPivotFormatConditions().get(formatIndex);
         FormatConditionCollection fcc = pfc.getFormatConditions();
         fcc.addArea(pivot.getDataBodyRange());
         int idx = fcc.addCondition(FormatConditionType.CELL_VALUE);
         FormatCondition fc = fcc.get(idx);
         fc.setFormula1("100");
         fc.setOperator(OperatorType.GREATER_OR_EQUAL);
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         pivot.refreshData();
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Methods

| Method | Description |
| --- | --- |
| [add(PivotTable pivotTable, int row, int column, String tableName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Adds a new PivotTable based on another PivotTable. |
| [add(PivotTable pivotTable, String destCellName, String tableName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Adds a new PivotTable based on another PivotTable. |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [add(String sourceData, int row, int column, String tableName)](#add-java.lang.String-int-int-java.lang.String-) | Adds a new PivotTable. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource)](#add-java.lang.String-int-int-java.lang.String-boolean-) | Adds a new PivotTable. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-int-int-java.lang.String-boolean-boolean-) | Adds a new PivotTable. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Adds a new PivotTable. |
| [add(String sourceData, String destCellName, String tableName, boolean useSameSource)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-) | Adds a new PivotTable. |
| [add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-) | Adds a new PivotTable. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-) | Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-) | Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source. |
| [clear()](#clear--) | Clears all pivot tables. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [dispose()](#dispose--) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the PivotTable report by index. |
| [get(int row, int column)](#get-int-int-) | Gets the PivotTable report by pivottable's position. |
| [get(String name)](#get-java.lang.String-) | Gets the PivotTable report by pivottable's name. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotTable pivotTable)](#remove-com.aspose.cells.PivotTable-) | Deletes the specified PivotTable and delete the PivotTable data |
| [remove(PivotTable pivotTable, boolean keepData)](#remove-com.aspose.cells.PivotTable-boolean-) | Deletes the specified PivotTable |
| [removeAt(int index)](#removeAt-int-) | Deletes the PivotTable at the specified index and delete the PivotTable data |
| [removeAt(int index, boolean keepData)](#removeAt-int-boolean-) | Deletes the PivotTable at the specified index |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivotTable, int row, int column, String tableName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivotTable, int row, int column, String tableName)
```


Adds a new PivotTable based on another PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | The source pivotTable. |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |

**Returns:**
int - The new added PivotTable index.
### add(PivotTable pivotTable, String destCellName, String tableName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivotTable, String destCellName, String tableName)
```


Adds a new PivotTable based on another PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | The source pivotTable. |
| destCellName | java.lang.String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |

**Returns:**
int - The new added PivotTable index.
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
### add(String sourceData, int row, int column, String tableName) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String sourceData, int row, int column, String tableName)
```


Adds a new PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |

**Returns:**
int - The new added cache index.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource) {#add-java.lang.String-int-int-java.lang.String-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource)
```


Adds a new PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |

**Returns:**
int - The new added cache index.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-int-int-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Adds a new PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |
| isXlsClassic | boolean | Indicates whether add classic pivot table of Excel 97-2003. |

**Returns:**
int - The new added cache index.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Adds a new PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | The data for the new PivotTable cache. |
| destCellName | java.lang.String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |

**Returns:**
int - The new added cache index.
### add(String sourceData, String destCellName, String tableName, boolean useSameSource) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public int add(String sourceData, String destCellName, String tableName, boolean useSameSource)
```


Adds a new PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | The data for the new PivotTable cache. |
| destCellName | java.lang.String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |

**Returns:**
int - The new added cache index.
### add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Adds a new PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| cell | java.lang.String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |
| isXlsClassic | boolean | Indicates whether add classic pivot table of Excel 97-2003. |

**Returns:**
int - The new added cache index.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)
```


Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String[] | The multiple consolidation ranges,such as \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | The pivot page field items. |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |

**Returns:**
int - The new added PivotTable index.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)
```


Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String[] | The multiple consolidation ranges,such as \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | The pivot page field items. |
| destCellName | java.lang.String | destCellName The name of the new PivotTable report. |
| tableName | java.lang.String | the name of the new PivotTable report. |

**Returns:**
int - The new added PivotTable index.
### clear() {#clear--}
```
public void clear()
```


Clears all pivot tables.

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
### dispose() {#dispose--}
```
public void dispose()
```


Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

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
public PivotTable get(int index)
```


Gets the PivotTable report by index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(int row, int column) {#get-int-int-}
```
public PivotTable get(int row, int column)
```


Gets the PivotTable report by pivottable's position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int |  |
| column | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(String name) {#get-java.lang.String-}
```
public PivotTable get(String name)
```


Gets the PivotTable report by pivottable's name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
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




### remove(PivotTable pivotTable) {#remove-com.aspose.cells.PivotTable-}
```
public void remove(PivotTable pivotTable)
```


Deletes the specified PivotTable and delete the PivotTable data

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |

### remove(PivotTable pivotTable, boolean keepData) {#remove-com.aspose.cells.PivotTable-boolean-}
```
public void remove(PivotTable pivotTable, boolean keepData)
```


Deletes the specified PivotTable

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| keepData | boolean | Whether to keep the PivotTable data |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Deletes the PivotTable at the specified index and delete the PivotTable data

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the position index in PivotTable collection |

### removeAt(int index, boolean keepData) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean keepData)
```


Deletes the PivotTable at the specified index

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the position index in PivotTable collection |
| keepData | boolean | Whether to keep the PivotTable data |

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

