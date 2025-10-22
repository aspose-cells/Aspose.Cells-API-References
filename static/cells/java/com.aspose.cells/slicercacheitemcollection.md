##SlicerCacheItemCollection
Represent the collection of SlicerCacheItem
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SlicerCacheItemCollection extends CollectionBase
```
Represent the collection of SlicerCacheItem
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
int slicerIndex = slicers.add(pivot, "E12", "fruit");
Slicer slicer = slicers.get(slicerIndex);
slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
SlicerCacheItemCollection items = slicer.getSlicerCache().getSlicerCacheItems();
//do your business
book.save("out.xlsx");
```
## Methods
| Method | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the SlicerCacheItem object by index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the count of the SlicerCacheItem. |
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
public SlicerCacheItem get(int index)
```
Gets the SlicerCacheItem object by index.
**Example**
```
SlicerCacheItem item = items.get(0);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
[SlicerCacheItem](../../com.aspose.cells/slicercacheitem)
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
Gets the count of the SlicerCacheItem.
**Example**
```
int count = items.getCount();
```
**Returns:**
int
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
