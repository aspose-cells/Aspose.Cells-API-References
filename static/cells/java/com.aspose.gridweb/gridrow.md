##GridRow
Encapsulates the object that represents a single picture in a spreadsheet.
**Inheritance:**
java.lang.Object
```
public class GridRow
```
Encapsulates the object that represents a single picture in a spreadsheet.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int column)](#get-int-) | Gets the cell. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Get the cell by specific index in the list. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Gets the first cell in the row. |
| [getHeight()](#getHeight--) | Gets the row height in unit of Points. |
| [getHidden()](#getHidden--) | Indicates whether the row is hidden. |
| [getIndex()](#getIndex--) | Gets the index of this row. |
| [getLastCell()](#getLastCell--) | Gets the last cell in the row. |
| [getLastDataCell()](#getLastDataCell--) | Gets the last cell in the row. |
| [getOutlineLevel()](#getOutlineLevel--) | Gets the outline level. |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Indicates whether the row contains any data |
| [iterator()](#iterator--) | Gets the cells enumerator |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeight(double value)](#setHeight-double-) | Sets the row height in unit of Points. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indicates whether the row is hidden. |
| [setOutlineLevel(byte value)](#setOutlineLevel-byte-) | Sets the outline level. |
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
### get(int column) {#get-int-}
```
public GridCell get(int column)
```
Gets the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | The column index |
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) -
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public GridCell getCellByIndex(int index)
```
Get the cell by specific index in the list.
**Remarks**
NOTE: This member is now obsolete. Instead,please use Row.GetEnumerator() method to iterate all cells in this row. This property will be removed 12 months later since February 2015. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position. |
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The Cell object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```
Gets the first cell in the row.
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHeight() {#getHeight--}
```
public double getHeight()
```
Gets the row height in unit of Points.
**Returns:**
double
### getHidden() {#getHidden--}
```
public boolean getHidden()
```
Indicates whether the row is hidden.
**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```
Gets the index of this row.
**Returns:**
int
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```
Gets the last cell in the row.
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastDataCell() {#getLastDataCell--}
```
public GridCell getLastDataCell()
```
Gets the last cell in the row.
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getOutlineLevel() {#getOutlineLevel--}
```
public byte getOutlineLevel()
```
Gets the outline level.
**Returns:**
byte
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```
Indicates whether the row contains any data
**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```
Gets the cells enumerator
**Returns:**
java.util.Iterator - The cells enumerator
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```
Sets the row height in unit of Points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```
Indicates whether the row is hidden.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOutlineLevel(byte value) {#setOutlineLevel-byte-}
```
public void setOutlineLevel(byte value)
```
Sets the outline level.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte |  |
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
