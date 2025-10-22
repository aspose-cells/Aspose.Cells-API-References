##RenameStrategy
Strategy option for duplicate names of columns.
**Inheritance:**
java.lang.Object
```
public final class RenameStrategy
```
Strategy option for duplicate names of columns.
**Remarks**
When processing data with headers, some scenarios require the headers to be no duplication for all columns. For example, when exporting data to a datatable and the header is required to be taken as datatable's column name, duplicated values of the header are invalid. For such kind of situations, user may determine how to handle them by specifying this strategy.
## Fields
| Field | Description |
| --- | --- |
| [DIGIT](#DIGIT) | Named with digit. |
| [EXCEPTION](#EXCEPTION) | Throws exception. |
| [LETTER](#LETTER) | Named with letter.. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DIGIT {#DIGIT}
```
public static final int DIGIT
```
Named with digit. Duplicated names will become ...1, ...2, etc.
### EXCEPTION {#EXCEPTION}
```
public static final int EXCEPTION
```
Throws exception.
### LETTER {#LETTER}
```
public static final int LETTER
```
Named with letter.. Duplicated names will become ...A, ...B, etc.
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
