##ControlMatchEntryType
Represents how a ListBox or ComboBox searches its list as the user types.
**Inheritance:**
java.lang.Object
```
public final class ControlMatchEntryType
```
Represents how a ListBox or ComboBox searches its list as the user types.
## Fields
| Field | Description |
| --- | --- |
| [COMPLETE](#COMPLETE) | As each character is typed, the control searches for an entry matching all characters entered. |
| [FIRST_LETTER](#FIRST-LETTER) | The control searches for the next entry that starts with the character entered. |
| [NONE](#NONE) | The list will not be searched when characters are typed. |
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
### COMPLETE {#COMPLETE}
```
public static final int COMPLETE
```
As each character is typed, the control searches for an entry matching all characters entered.
### FIRST_LETTER {#FIRST-LETTER}
```
public static final int FIRST_LETTER
```
The control searches for the next entry that starts with the character entered. Repeatedly typing the same letter cycles through all entries beginning with that letter.
### NONE {#NONE}
```
public static final int NONE
```
The list will not be searched when characters are typed.
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
