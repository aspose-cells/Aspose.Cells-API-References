---
title: "RevisionFormat"
second_title: "Aspose.Cells for Java API 参考"
description: "表示有关格式更改的信息的修订记录。"
type: docs
url: /zh/java/com.aspose.cells/revisionformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionFormat extends Revision
```

表示有关格式更改的信息的修订记录。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | 此格式应用的范围。 |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | 获取此修订的编号。 |
| [getStyle()](#getStyle--) | 获取已应用的样式。 |
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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


此格式应用的范围。

**Returns:**
com.aspose.cells.CellArea[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getId() {#getId--}
```
public int getId()
```


获取此修订的编号。

**Remarks**

零表示此修订不包含 ID。

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


获取已应用的样式。

**Returns:**
[Style](../../com.aspose.cells/style)
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

