##RevisionInsertSheet
Represents a revision record of a sheet that was inserted.
**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionInsertSheet extends Revision
```
Represents a revision record of a sheet that was inserted.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Gets the action type of the revision. |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | Gets the number of this revision. |
| [getName()](#getName--) | Gets the name of the worksheet. |
| [getSheetPosition()](#getSheetPosition--) | Gets the zero based position of the new sheet in the sheet tab bar. |
| [getType()](#getType--) | Gets the type of revision. |
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
Gets the action type of the revision.
See [RevisionActionType](../../com.aspose.cells/revisionactiontype).
**Returns:**
int
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
### getName() {#getName--}
```
public String getName()
```
Gets the name of the worksheet.
**Returns:**
java.lang.String
### getSheetPosition() {#getSheetPosition--}
```
public int getSheetPosition()
```
Gets the zero based position of the new sheet in the sheet tab bar.
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
