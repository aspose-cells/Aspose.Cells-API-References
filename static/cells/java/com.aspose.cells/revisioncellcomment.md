##RevisionCellComment
Represents a revision record of a cell comment change.
**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellComment extends Revision
```
Represents a revision record of a cell comment change.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Gets the action type of the revision. |
| [getCellName()](#getCellName--) | Gets the name of the cell. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Gets the column index of the which contains a comment. |
| [getId()](#getId--) | Gets the number of this revision. |
| [getNewLength()](#getNewLength--) | Gets Length of the comment before this revision was made. |
| [getOldLength()](#getOldLength--) | Gets Length of the comment text added in this revision. |
| [getRow()](#getRow--) | Gets the row index of the which contains a comment. |
| [getType()](#getType--) | Gets the type of revision. |
| [getWorksheet()](#getWorksheet--) | Gets the worksheet. |
| [hashCode()](#hashCode--) |  |
| [isOldComment()](#isOldComment--) | Indicates whether it's an old comment. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellName(String value)](#setCellName-java.lang.String-) | Gets the name of the cell. |
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
Gets the action type of the revision.
See [RevisionActionType](../../com.aspose.cells/revisionactiontype).
**Returns:**
int
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
Gets the column index of the which contains a comment.
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
### getNewLength() {#getNewLength--}
```
public int getNewLength()
```
Gets Length of the comment before this revision was made.
**Returns:**
int
### getOldLength() {#getOldLength--}
```
public int getOldLength()
```
Gets Length of the comment text added in this revision.
**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```
Gets the row index of the which contains a comment.
**Returns:**
int
### getType() {#getType--}
```
public int getType()
```
Gets the type of revision.
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
### isOldComment() {#isOldComment--}
```
public boolean isOldComment()
```
Indicates whether it's an old comment.
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
### setCellName(String value) {#setCellName-java.lang.String-}
```
public void setCellName(String value)
```
Gets the name of the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
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
