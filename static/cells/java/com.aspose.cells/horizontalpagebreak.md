##HorizontalPageBreak
Encapsulates the object that represents a horizontal page break.
**Inheritance:**
java.lang.Object
```
public class HorizontalPageBreak
```
Encapsulates the object that represents a horizontal page break.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.getWorksheets().get(0);
//Add a page break at cell Y30
int Index = worksheet.getHorizontalPageBreaks().add("Y30");
//get the newly added horizontal page break
HorizontalPageBreak hPageBreak = worksheet.getHorizontalPageBreaks().get(Index);
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | Gets the end column index of this horizontal page break. |
| [getRow()](#getRow--) | Gets the zero based row index. |
| [getStartColumn()](#getStartColumn--) | Gets the start column index of this horizontal page break. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```
Gets the end column index of this horizontal page break.
**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```
Gets the zero based row index.
**Returns:**
int
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```
Gets the start column index of this horizontal page break.
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
