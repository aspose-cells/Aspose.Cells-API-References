---
title: MemorySetting
second_title: Aspose.Cells for Java API Reference
description: Memory usage modes for cells data model.
type: docs
url: /java/com.aspose.cells/memorysetting/
---

**Inheritance:**
java.lang.Object
```
public final class MemorySetting
```

Memory usage modes for cells data model.
## Fields

| Field | Description |
| --- | --- |
| [MEMORY_PREFERENCE](#MEMORY-PREFERENCE) | Memory performance preferrable. |
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
### MEMORY_PREFERENCE {#MEMORY-PREFERENCE}
```
public static final int MEMORY_PREFERENCE
```


Memory performance preferrable.

**Remarks**

With this mode the cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing it randomly, This option is available since v 8.0.0.

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

