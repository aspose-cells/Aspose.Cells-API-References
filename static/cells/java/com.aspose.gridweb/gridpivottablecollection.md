##GridPivotTableCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object
```
public class GridPivotTableCollection
```
Encapsulates a collection of [GridPivotTable](../../com.aspose.gridweb/gridpivottable) objects.
## Methods
| Method | Description |
| --- | --- |
| [add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)](#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Adds a new PivotTable cache to a PivotCaches collection. |
| [add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-) | Adds a new PivotTable cache to a PivotCaches collection. |
| [add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Adds a new PivotTable cache to a PivotCaches collection. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Adds a new PivotTable cache to a PivotCaches collection. |
| [clear()](#clear--) | Clears all PivotTables. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [GridPivotTable](../../com.aspose.gridweb/gridpivottable) element at the specified index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the size of enumerator |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Remove the PivotTable at the specified index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName) {#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)
```
Adds a new PivotTable cache to a PivotCaches collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | The source work sheet. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | The area in the source worksheet. |
| destCellName | java.lang.String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |
**Returns:**
int - The new added cache index.
### add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)
```
Adds a new PivotTable cache to a PivotCaches collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| worksheetname | java.lang.String | The name of the source worksheet. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | The area in the source worksheet. |
| destRow | int | The row of the cell in the upper-left corner of the PivotTable report's destination range. |
| destCol | int | The column of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |
**Returns:**
int - The new added cache index.
### add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)
```
Adds a new PivotTable cache to a PivotCaches collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| worksheetname | java.lang.String | The name of the source worksheet. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | The area in the source worksheet. |
| destCellName | java.lang.String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |
**Returns:**
int - The new added cache index.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```
Adds a new PivotTable cache to a PivotCaches collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| destCellName | java.lang.String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | java.lang.String | The name of the new PivotTable report. |
**Returns:**
int - The new added cache index.
### clear() {#clear--}
```
public void clear()
```
Clears all PivotTables.
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
public GridPivotTable get(int index)
```
Gets the [GridPivotTable](../../com.aspose.gridweb/gridpivottable) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[GridPivotTable](../../com.aspose.gridweb/gridpivottable) - The element at the specified index.
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
Gets the size of enumerator
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
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
Remove the PivotTable at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
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
