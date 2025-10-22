##DirectoryType
Represents the directory  type of the file name.
**Inheritance:**
java.lang.Object
```
public final class DirectoryType
```
Represents the directory type of the file name.
## Fields
| Field | Description |
| --- | --- |
| [DOWN_DIRECTORY](#DOWN-DIRECTORY) | Indicates that the source workbook is in a subdirectory of the current directory. |
| [SAME_VOLUME](#SAME-VOLUME) | Indicates that the source workbook is on the same drive as the dependent workbook (the drive letter is omitted) |
| [UP_DIRECTORY](#UP-DIRECTORY) | Indicates that the source workbook is in the parent directory of the current directory. |
| [VOLUME](#VOLUME) | Represents an MS-DOS drive letter. |
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
### DOWN_DIRECTORY {#DOWN-DIRECTORY}
```
public static final int DOWN_DIRECTORY
```
Indicates that the source workbook is in a subdirectory of the current directory.
### SAME_VOLUME {#SAME-VOLUME}
```
public static final int SAME_VOLUME
```
Indicates that the source workbook is on the same drive as the dependent workbook (the drive letter is omitted)
### UP_DIRECTORY {#UP-DIRECTORY}
```
public static final int UP_DIRECTORY
```
Indicates that the source workbook is in the parent directory of the current directory.
### VOLUME {#VOLUME}
```
public static final int VOLUME
```
Represents an MS-DOS drive letter. It is followed by the drive letter. Or UNC file names, such as \\\\server\\share\\myfile.xls
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
