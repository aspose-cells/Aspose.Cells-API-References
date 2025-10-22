##GridHyperlinkCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object
```
public class GridHyperlinkCollection
```
Encapsulates a collection of [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) objects.
## Methods
| Method | Description |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | Adds a hyperlink to a specified cell or a range of cells. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | Adds a hyperlink to a specified cell or a range of cells. |
| [add(String cellName, String address)](#add-java.lang.String-java.lang.String-) | Adds a hyperlink to a specified cell . |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Adds a hyperlink to a specified cell or a range of cells. |
| [clear()](#clear--) | Clears all hyperlinks. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) element at the specified index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the size of enumerator |
| [getHyperlink(GridCell cell)](#getHyperlink-com.aspose.gridweb.GridCell-) | Gets the cell's Hyperlink object. |
| [getHyperlink(int row, int column)](#getHyperlink-int-int-) | Gets the cell's Hyperlink object. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(GridCellArea area)](#remove-com.aspose.gridweb.GridCellArea-) | Remove the hyperlink at the specified area. |
| [removeAt(int index)](#removeAt-int-) | Remove the hyperlink at the specified index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```
Adds a hyperlink to a specified cell or a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | First row of the hyperlink range. |
| firstColumn | int | First column of the hyperlink range. |
| totalRows | int | Number of rows in this hyperlink range. |
| totalColumns | int | Number of columns of this hyperlink range. |
| address | java.lang.String | Address of the hyperlink. |
**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) object index.
### add(String cellName, int totalRows, int totalColumns, String address) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String cellName, int totalRows, int totalColumns, String address)
```
Adds a hyperlink to a specified cell or a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name. |
| totalRows | int | Number of rows in this hyperlink range. |
| totalColumns | int | Number of columns of this hyperlink range. |
| address | java.lang.String | Address of the hyperlink. |
**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) object index.
### add(String cellName, String address) {#add-java.lang.String-java.lang.String-}
```
public int add(String cellName, String address)
```
Adds a hyperlink to a specified cell .
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name. |
| address | java.lang.String | Address of the hyperlink. |
**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) object index.
### add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip) {#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)
```
Adds a hyperlink to a specified cell or a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | java.lang.String | The top-left cell of the range. |
| endCellName | java.lang.String | The bottom-right cell of the range. |
| address | java.lang.String | Address of the hyperlink. |
| textToDisplay | java.lang.String | The text to be displayed for the specified hyperlink. |
| screenTip | java.lang.String | The screenTip text for the specified hyperlink. |
**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) object index.
### clear() {#clear--}
```
public void clear()
```
Clears all hyperlinks.
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
public GridHyperlink get(int index)
```
Gets the [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - The element at the specified index.
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
### getHyperlink(GridCell cell) {#getHyperlink-com.aspose.gridweb.GridCell-}
```
public GridHyperlink getHyperlink(GridCell cell)
```
Gets the cell's Hyperlink object. If there is no Hyperlink of the cell, returns null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [GridCell](../../com.aspose.gridweb/gridcell) | The GridCell object. |
**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
### getHyperlink(int row, int column) {#getHyperlink-int-int-}
```
public GridHyperlink getHyperlink(int row, int column)
```
Gets the cell's Hyperlink object. If there is no Hyperlink of the cell, returns null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row of the cell. |
| column | int | The column of the cell. |
**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
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
### remove(GridCellArea area) {#remove-com.aspose.gridweb.GridCellArea-}
```
public void remove(GridCellArea area)
```
Remove the hyperlink at the specified area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | The area which contains hyperlink. |
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Remove the hyperlink at the specified index.
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
