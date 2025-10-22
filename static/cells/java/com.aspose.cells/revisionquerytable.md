##RevisionQueryTable
Represents a revision of a query table field change.
**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionQueryTable extends Revision
```
Represents a revision of a query table field change.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellArea()](#getCellArea--) | Gets the location of the affected query table. |
| [getClass()](#getClass--) |  |
| [getFieldId()](#getFieldId--) | Gets ID of the specific query table field that was removed. |
| [getId()](#getId--) | Gets the number of this revision. |
| [getType()](#getType--) | Represents the type of the revision. |
| [getWorksheet()](#getWorksheet--) | Gets the worksheet. |
| [hashCode()](#hashCode--) |  |
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
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```
Gets the location of the affected query table.
**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getFieldId() {#getFieldId--}
```
public int getFieldId()
```
Gets ID of the specific query table field that was removed.
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
### getType() {#getType--}
```
public int getType()
```
Represents the type of the revision.
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
