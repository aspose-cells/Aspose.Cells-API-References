---
title: "RowColumnEventArgs"
second_title: "Aspose.Cells for Java API 参考"
description: "为行/列事件提供数据。"
type: docs
url: /zh/java/com.aspose.gridweb/rowcolumneventargs/
---

**Inheritance:**
java.lang.Object
```
public class RowColumnEventArgs
```

为行/列事件提供数据。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgument()](#getArgument--) | 事件的参数。 |
| [getClass()](#getClass--) |  |
| [getNum()](#getNum--) | 行或列的编号，从零开始。 |
| [getType()](#getType--) | 行或列的类型。 |
| [hashCode()](#hashCode--) |  |
| [isCancel()](#isCancel--) | 我们是否取消操作。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rejectOperation()](#rejectOperation--) | 在 RowDeleting/ColumnDeleting 事件处理程序中调用此方法以取消删除操作。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArgument() {#getArgument--}
```
public Object getArgument()
```


事件的参数。

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getNum() {#getNum--}
```
public int getNum()
```


行或列的编号，从零开始。

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


行或列的类型。

参见 [RowColumnType](../../com.aspose.gridweb/rowcolumntype)。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCancel() {#isCancel--}
```
public boolean isCancel()
```


我们是否取消操作。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### rejectOperation() {#rejectOperation--}
```
public void rejectOperation()
```


在 RowDeleting/ColumnDeleting 事件处理程序中调用此方法以取消删除操作。

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

