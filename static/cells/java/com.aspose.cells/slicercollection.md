##SlicerCollection
Specifies the collection of all the Slicer objects on the specified worksheet.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SlicerCollection extends CollectionBase
```
Specifies the collection of all the Slicer objects on the specified worksheet.
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
pivot.refreshData();
pivot.calculateData();
SlicerCollection slicers = sheet.getSlicers();
int tableIndex = sheet.getListObjects().add("A1", "C9", true);
ListObject table = sheet.getListObjects().get(tableIndex);
//do your business
book.save("out.xlsx");
```
## Methods
| Method | Description |
| --- | --- |
| [add(ListObject table, ListColumn listColumn, int row, int column)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-) | Add a new Slicer using ListObjet as data source |
| [add(ListObject table, ListColumn listColumn, String destCellName)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-) | Add a new Slicer using ListObjet as data source |
| [add(ListObject table, int index, String destCellName)](#add-com.aspose.cells.ListObject-int-java.lang.String-) | Add a new Slicer using ListObjet as data source |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | Add a new Slicer using PivotTable as data source |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | Add a new Slicer using PivotTable as data source |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Add a new Slicer using PivotTable as data source |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | Add a new Slicer using PivotTable as data source |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | Add a new Slicer using PivotTable as data source |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Add a new Slicer using PivotTable as data source |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [clear()](#clear--) | Clear all Slicers. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the Slicer by index. |
| [get(String name)](#get-java.lang.String-) | Gets the Slicer by slicer's name. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Slicer slicer)](#remove-com.aspose.cells.Slicer-) | Remove the specified Slicer |
| [removeAt(int index)](#removeAt-int-) | Deletes the Slicer at the specified index |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ListObject table, ListColumn listColumn, int row, int column) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-}
```
public int add(ListObject table, ListColumn listColumn, int row, int column)
```
Add a new Slicer using ListObjet as data source
**Example**
```
slicers.add(table, table.getListColumns().get(1), 38, 12);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject object |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | The ListColumn in ListObject.ListColumns |
| row | int | Row index of the cell in the upper-left corner of the Slicer range. |
| column | int | Column index of the cell in the upper-left corner of the Slicer range. |
**Returns:**
int - The new add Slicer index
### add(ListObject table, ListColumn listColumn, String destCellName) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-}
```
public int add(ListObject table, ListColumn listColumn, String destCellName)
```
Add a new Slicer using ListObjet as data source
**Example**
```
slicers.add(table, table.getListColumns().get(1), "I38");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject object |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | The ListColumn in ListObject.ListColumns |
| destCellName | java.lang.String | The cell in the upper-left corner of the Slicer range. |
**Returns:**
int - The new add Slicer index
### add(ListObject table, int index, String destCellName) {#add-com.aspose.cells.ListObject-int-java.lang.String-}
```
public int add(ListObject table, int index, String destCellName)
```
Add a new Slicer using ListObjet as data source
**Example**
```
slicers.add(table, 1, "E38");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject object |
| index | int | The index of ListColumn in ListObject.ListColumns |
| destCellName | java.lang.String | The cell in the upper-left corner of the Slicer range. |
**Returns:**
int - The new add Slicer index
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```
Add a new Slicer using PivotTable as data source
**Example**
```
slicers.add(pivot, 3, 12, pivot.getBaseFields().get(0));
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Slicer range. |
| column | int | Column index of the cell in the upper-left corner of the Slicer range. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | The PivotField in PivotTable.BaseFields |
**Returns:**
int - The new add Slicer index
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```
Add a new Slicer using PivotTable as data source
**Example**
```
slicers.add(pivot, 20, 8, 0);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Slicer range. |
| column | int | Column index of the cell in the upper-left corner of the Slicer range. |
| baseFieldIndex | int | The index of PivotField in PivotTable.BaseFields |
**Returns:**
int - The new add Slicer index
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```
Add a new Slicer using PivotTable as data source
**Example**
```
slicers.add(pivot, 20, 12, "fruit");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Slicer range. |
| column | int | Column index of the cell in the upper-left corner of the Slicer range. |
| baseFieldName | java.lang.String | The name of PivotField in PivotTable.BaseFields |
**Returns:**
int - The new add Slicer index
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```
Add a new Slicer using PivotTable as data source
**Example**
```
slicers.add(pivot, "I3", pivot.getBaseFields().get(0));
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| destCellName | java.lang.String | The cell in the upper-left corner of the Slicer range. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | The PivotField in PivotTable.BaseFields |
**Returns:**
int - The new add Slicer index
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```
Add a new Slicer using PivotTable as data source
**Example**
```
slicers.add(pivot, "E20", 0);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| destCellName | java.lang.String | The cell in the upper-left corner of the Slicer range. |
| baseFieldIndex | int | The index of PivotField in PivotTable.BaseFields |
**Returns:**
int - The new add Slicer index
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```
Add a new Slicer using PivotTable as data source
**Example**
```
slicers.add(pivot, "E3", "fruit");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| destCellName | java.lang.String | The cell in the upper-left corner of the Slicer range. |
| baseFieldName | java.lang.String | The name of PivotField in PivotTable.BaseFields |
**Returns:**
int - The new add Slicer index
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
Clear all Slicers.
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
public Slicer get(int index)
```
Gets the Slicer by index.
**Example**
```
Slicer slicerByIndex = slicers.get(0);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
[Slicer](../../com.aspose.cells/slicer)
### get(String name) {#get-java.lang.String-}
```
public Slicer get(String name)
```
Gets the Slicer by slicer's name.
**Example**
```
Slicer slicerByName = slicers.get("fruit");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |
**Returns:**
[Slicer](../../com.aspose.cells/slicer)
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
### remove(Slicer slicer) {#remove-com.aspose.cells.Slicer-}
```
public void remove(Slicer slicer)
```
Remove the specified Slicer
**Example**
```
Slicer delSlicer = slicers.get(0);
slicers.remove(delSlicer);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| slicer | [Slicer](../../com.aspose.cells/slicer) | The Slicer object |
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Deletes the Slicer at the specified index
**Example**
```
slicers.removeAt(1);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position index in Slicer collection |
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
