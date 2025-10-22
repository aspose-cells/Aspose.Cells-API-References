##CoWorkUserPermission
represent the user permission  in collaboration mode.only available in java version now will be available in .netython version in future.
**Inheritance:**
java.lang.Object
```
public final class CoWorkUserPermission
```
represent the user permission in collaboration mode.only available in java version now, will be available in .net/python version in future.
## Fields
| Field | Description |
| --- | --- |
| [ADMIN](#ADMIN) | Administrator permission,User has full access including management operations |
| [DOWNLOAD](#DOWNLOAD) | Download permission,User can view,edit and download the content to local storage |
| [EDITABLE](#EDITABLE) | Editable permission,User can view and edit the content |
| [READ_ONLY](#READ-ONLY) | Read-only permission,User can only view the content but cannot make any modifications |
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
### ADMIN {#ADMIN}
```
public static final int ADMIN
```
Administrator permission,User has full access including management operations
### DOWNLOAD {#DOWNLOAD}
```
public static final int DOWNLOAD
```
Download permission,User can view,edit and download the content to local storage
### EDITABLE {#EDITABLE}
```
public static final int EDITABLE
```
Editable permission,User can view and edit the content
### READ_ONLY {#READ-ONLY}
```
public static final int READ_ONLY
```
Read-only permission,User can only view the content but cannot make any modifications
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
