##RevisionCellChange
Represents the revision that changing cells.
**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellChange extends Revision
```
Represents the revision that changing cells.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellName()](#getCellName--) | Gets the name of the cell. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Gets the column index of the cell. |
| [getId()](#getId--) | Gets the number of this revision. |
| [getNewFormula()](#getNewFormula--) | Gets the old formula. |
| [getNewStyle()](#getNewStyle--) | Gets the new style of the cell. |
| [getNewValue()](#getNewValue--) | Gets new value of the cell. |
| [getOldFormula()](#getOldFormula--) | Gets the old formula. |
| [getOldStyle()](#getOldStyle--) | Gets the old style of the cell. |
| [getOldValue()](#getOldValue--) | Gets old value of the cell. |
| [getRow()](#getRow--) | Gets the row index of the cell. |
| [getType()](#getType--) | Represents the type of revision. |
| [getWorksheet()](#getWorksheet--) | Gets the worksheet. |
| [hashCode()](#hashCode--) |  |
| [isNewFormatted()](#isNewFormatted--) | Indicates whether this cell is new formatted. |
| [isOldFormatted()](#isOldFormatted--) | Indicates whether this cell is old formatted. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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
### getCellName() {#getCellName--}
```
public String getCellName()
```
Gets the name of the cell.
**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```
Gets the column index of the cell.
**Returns:**
int
### getId() {#getId--}
```
public int getId()
```
Gets the number of this revision.
**Remarks**
Zero means this revision does not contains id.
**Returns:**
int
### getNewFormula() {#getNewFormula--}
```
public String getNewFormula()
```
Gets the old formula.
**Returns:**
java.lang.String
### getNewStyle() {#getNewStyle--}
```
public Style getNewStyle()
```
Gets the new style of the cell.
**Returns:**
[Style](../../com.aspose.cells/style)
### getNewValue() {#getNewValue--}
```
public Object getNewValue()
```
Gets new value of the cell.
**Returns:**
java.lang.Object
### getOldFormula() {#getOldFormula--}
```
public String getOldFormula()
```
Gets the old formula.
**Returns:**
java.lang.String
### getOldStyle() {#getOldStyle--}
```
public Style getOldStyle()
```
Gets the old style of the cell.
**Returns:**
[Style](../../com.aspose.cells/style)
### getOldValue() {#getOldValue--}
```
public Object getOldValue()
```
Gets old value of the cell.
**Returns:**
java.lang.Object
### getRow() {#getRow--}
```
public int getRow()
```
Gets the row index of the cell.
**Returns:**
int
### getType() {#getType--}
```
public int getType()
```
Represents the type of revision.
See [RevisionType](../../com.aspose.cells/revisiontype).
**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```
Gets the worksheet.
**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isNewFormatted() {#isNewFormatted--}
```
public boolean isNewFormatted()
```
Indicates whether this cell is new formatted.
**Returns:**
boolean
### isOldFormatted() {#isOldFormatted--}
```
public boolean isOldFormatted()
```
Indicates whether this cell is old formatted.
**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
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
