---
title: "RevisionCellChange"
second_title: "Aspose.Cells for Java API 参考"
description: "表示更改单元格的修订。"
type: docs
url: /zh/java/com.aspose.cells/revisioncellchange/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellChange extends Revision
```

表示更改单元格的修订。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellName()](#getCellName--) | 获取单元格的名称。 |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | 获取单元格的列索引。 |
| [getId()](#getId--) | 获取此修订的编号。 |
| [getNewFormula()](#getNewFormula--) | 获取旧公式。 |
| [getNewStyle()](#getNewStyle--) | 获取单元格的新样式。 |
| [getNewValue()](#getNewValue--) | 获取单元格的新值。 |
| [getOldFormula()](#getOldFormula--) | 获取旧公式。 |
| [getOldStyle()](#getOldStyle--) | 获取单元格的旧样式。 |
| [getOldValue()](#getOldValue--) | 获取单元格的旧值。 |
| [getRow()](#getRow--) | 获取单元格的行索引。 |
| [getType()](#getType--) | 表示修订的类型。 |
| [getWorksheet()](#getWorksheet--) | 获取工作表。 |
| [hashCode()](#hashCode--) |  |
| [isNewFormatted()](#isNewFormatted--) | 指示此单元格是否已新格式化。 |
| [isOldFormatted()](#isOldFormatted--) | 指示此单元格是否为旧格式。 |
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


获取单元格的列索引。

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
### getNewFormula() {#getNewFormula--}
```
public String getNewFormula()
```


获取旧公式。

**Returns:**
java.lang.String
### getNewStyle() {#getNewStyle--}
```
public Style getNewStyle()
```


获取单元格的新样式。

**Returns:**
[Style](../../com.aspose.cells/style)
### getNewValue() {#getNewValue--}
```
public Object getNewValue()
```


获取单元格的新值。

**Returns:**
java.lang.Object
### getOldFormula() {#getOldFormula--}
```
public String getOldFormula()
```


获取旧公式。

**Returns:**
java.lang.String
### getOldStyle() {#getOldStyle--}
```
public Style getOldStyle()
```


获取单元格的旧样式。

**Returns:**
[Style](../../com.aspose.cells/style)
### getOldValue() {#getOldValue--}
```
public Object getOldValue()
```


获取单元格的旧值。

**Returns:**
java.lang.Object
### getRow() {#getRow--}
```
public int getRow()
```


获取单元格的行索引。

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


表示修订的类型。

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
### isNewFormatted() {#isNewFormatted--}
```
public boolean isNewFormatted()
```


指示此单元格是否已新格式化。

**Returns:**
boolean
### isOldFormatted() {#isOldFormatted--}
```
public boolean isOldFormatted()
```


指示此单元格是否为旧格式。

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

