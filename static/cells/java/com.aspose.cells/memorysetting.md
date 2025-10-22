##MemorySetting
Memory usage modes for cells data model.
**Inheritance:**
java.lang.Object
```
public final class MemorySetting
```
Memory usage modes for cells data model.
## Fields
| Field | Description |
| --- | --- |
| [FILE_CACHE](#FILE-CACHE) | Memory performance preferable and using file instead of memory to maintain the cells data. |
| [MEMORY_PREFERENCE](#MEMORY-PREFERENCE) | Memory performance preferable. |
| [NORMAL](#NORMAL) | Default mode for cells model. |
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
### FILE_CACHE {#FILE-CACHE}
```
public static final int FILE_CACHE
```
Memory performance preferable and using file instead of memory to maintain the cells data.
**Remarks**
With this mode the cells data will be maintained in compact format and the major part of the data will be maintained in temporary file instead of memory. So when comparing with [MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) mode, this mode may decrease the memory cost more, but the IO operations for accessing cells data also will cause higher time cost.
This option is available since v25.7.0.
| Some notable limits and recommended operations when using this mode:                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| When this mode is used for any worksheet in one workbook, [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) should be called at the end of work to release all resources such as the temporary files.                                                                                                                                                                                                                                                                                                  |
| Randomly accessing cells will give poor performance because data needs to be read randomly and repeatedly(so the pointer in the file will be changed accordingly and IO operations will be required repeatedly). If possible, please always access the data sequentially(row by row).                                                                                                                                                                                                                                |
| When the data of one row/cell be changed, data of other cells/rows may also be influenced(such as the data be shifted/moved to other places to allocated enough spaces for the changed data). So every change of every data requires synchronization of other existing objects(such as Row or Cell object). So, to get better performance, please do not maintain multiple Rows/Cells at the same time. Processing them one by one will reduce the data synchronization for them so the performance can be improved. |
### MEMORY_PREFERENCE {#MEMORY-PREFERENCE}
```
public static final int MEMORY_PREFERENCE
```
Memory performance preferable.
**Remarks**
With this mode the cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing it randomly.
This option is available since v8.0.0.
### NORMAL {#NORMAL}
```
public static final int NORMAL
```
Default mode for cells model.
**Remarks**
This mode is applied for all versions.
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
