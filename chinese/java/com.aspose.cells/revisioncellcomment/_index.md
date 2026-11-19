---
title: "RevisionCellComment"
second_title: "Aspose.Cells for Java API 参考"
description: "表示单元格批注更改的修订记录。"
type: docs
url: /zh/java/com.aspose.cells/revisioncellcomment/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellComment extends Revision
```

表示单元格批注更改的修订记录。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | 获取修订的操作类型。 |
| [getCellName()](#getCellName--) | 获取单元格的名称。 |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | 获取包含注释的列索引。 |
| [getId()](#getId--) | 获取此修订的编号。 |
| [getNewLength()](#getNewLength--) | 获取此修订之前的注释长度。 |
| [getOldLength()](#getOldLength--) | 获取此修订中添加的注释文本长度。 |
| [getRow()](#getRow--) | 获取包含注释的行索引。 |
| [getType()](#getType--) | 获取修订的类型。 |
| [getWorksheet()](#getWorksheet--) | 获取工作表。 |
| [hashCode()](#hashCode--) |  |
| [isOldComment()](#isOldComment--) | 指示它是否是旧注释。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellName(String value)](#setCellName-java.lang.String-) | 获取单元格的名称。 |
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


获取修订的操作类型。

参见 [RevisionActionType](../../com.aspose.cells/revisionactiontype)。

**Returns:**
int
### getCellName() {#getCellName--}
```
public String getCellName()
```


获取单元格的名称。

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


获取包含注释的列索引。

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


获取此修订的编号。

**Remarks**

零表示此修订不包含 ID。

**Returns:**
int
### getNewLength() {#getNewLength--}
```
public int getNewLength()
```


获取此修订之前的注释长度。

**Returns:**
int
### getOldLength() {#getOldLength--}
```
public int getOldLength()
```


获取此修订中添加的注释文本长度。

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


获取包含注释的行索引。

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
### isOldComment() {#isOldComment--}
```
public boolean isOldComment()
```


指示它是否是旧注释。

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




### setCellName(String value) {#setCellName-java.lang.String-}
```
public void setCellName(String value)
```


获取单元格的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

