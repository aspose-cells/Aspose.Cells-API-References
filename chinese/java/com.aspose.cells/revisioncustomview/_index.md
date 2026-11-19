---
title: "RevisionCustomView"
second_title: "Aspose.Cells for Java API 参考"
description: "表示向工作簿添加或删除自定义视图的修订记录"
type: docs
url: /zh/java/com.aspose.cells/revisioncustomview/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCustomView extends Revision
```

表示向工作簿添加或删除自定义视图的修订记录
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | 获取操作的类型。 |
| [getClass()](#getClass--) |  |
| [getGuid()](#getGuid--) | 获取自定义视图的全局唯一标识符。 |
| [getId()](#getId--) | 获取此修订的编号。 |
| [getType()](#getType--) | 获取修订的类型。 |
| [getWorksheet()](#getWorksheet--) | 获取工作表。 |
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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getActionType() {#getActionType--}
```
public int getActionType()
```


获取操作的类型。

参见 [RevisionActionType](../../com.aspose.cells/revisionactiontype)。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


获取自定义视图的全局唯一标识符。

**Returns:**
java.util.UUID
### getId() {#getId--}
```
public int getId()
```


获取此修订的编号。

**Remarks**

零表示此修订不包含 ID。

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


获取修订的类型。

查看 [RevisionType](../../com.aspose.cells/revisiontype)。

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


获取工作表。

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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

