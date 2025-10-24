##VerticalPageBreak
Encapsulates the object that represents a vertical page break.
**Inheritance:**
java.lang.Object
```
public class VerticalPageBreak
```
Encapsulates the object that represents a vertical page break.
**Example**
```
Workbook excel = new Workbook();
//Add a pagebreak at G5
excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Gets the column index of the vertical page break. |
| [getEndRow()](#getEndRow--) | Gets the end row index of the vertical page break. |
| [getStartRow()](#getStartRow--) | Gets the start row index of the vertical page break. |
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
### getColumn() {#getColumn--}
```
public int getColumn()
```
Gets the column index of the vertical page break.
**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```
Gets the end row index of the vertical page break.
**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```
Gets the start row index of the vertical page break.
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
