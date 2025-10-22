##RevisionInsertDelete
Represents a revision record of a row/column insert/delete action.
**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionInsertDelete extends Revision
```
Represents a revision record of a row/column insert/delete action.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Gets the action type of this revision. |
| [getCellArea()](#getCellArea--) | Gets the inserting/deleting range. |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | Gets the number of this revision. |
| [getRevisions()](#getRevisions--) | Gets revision list by this operation. |
| [getType()](#getType--) | Represents the type of revision. |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```
Gets the action type of this revision.
See [RevisionActionType](../../com.aspose.cells/revisionactiontype).
**Returns:**
int
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```
Gets the inserting/deleting range.
**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getId() {#getId--}
```
public int getId()
```
Gets the number of this revision.
**Remarks**
Zero means this revision does not contains id.
**Returns:**
int
### getRevisions() {#getRevisions--}
```
public RevisionCollection getRevisions()
```
Gets revision list by this operation.
**Returns:**
[RevisionCollection](../../com.aspose.cells/revisioncollection)
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
