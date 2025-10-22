##PaneStateType
Represents state of the sheets pane.
**Inheritance:**
java.lang.Object
```
public final class PaneStateType
```
Represents state of the sheet's pane.
## Fields
| Field | Description |
| --- | --- |
| [FROZEN](#FROZEN) | Panes are frozen, but were not before being frozen. |
| [FROZEN_SPLIT](#FROZEN-SPLIT) | Panes are frozen and were split before being frozen. |
| [NORMAL](#NORMAL) | Panes are not frozen and not split. |
| [SPLIT](#SPLIT) | Panes are split, but not frozen. |
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
### FROZEN {#FROZEN}
```
public static final int FROZEN
```
Panes are frozen, but were not before being frozen.
### FROZEN_SPLIT {#FROZEN-SPLIT}
```
public static final int FROZEN_SPLIT
```
Panes are frozen and were split before being frozen.
### NORMAL {#NORMAL}
```
public static final int NORMAL
```
Panes are not frozen and not split.
### SPLIT {#SPLIT}
```
public static final int SPLIT
```
Panes are split, but not frozen.
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
