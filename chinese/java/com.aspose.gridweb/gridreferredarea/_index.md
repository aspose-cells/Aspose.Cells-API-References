---
title: "GridReferredArea"
second_title: "Aspose.Cells for Java API 参考"
description: "表示公式引用的对象。"
type: docs
url: /zh/java/com.aspose.gridweb/gridreferredarea/
---

**Inheritance:**
java.lang.Object
```
public class GridReferredArea
```

表示公式引用的对象。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | 区域的结束列。 |
| [getEndRow()](#getEndRow--) | 区域的结束行。 |
| [getExternalFileName()](#getExternalFileName--) | this.KeepedRels = source.KeepedRels; |
| [getSheetName()](#getSheetName--) | 指示所在的工作表 |
| [getStartColumn()](#getStartColumn--) | 区域的起始列。 |
| [getStartRow()](#getStartRow--) | 区域的起始行。 |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | 获取相对于此区域左上角给定偏移量的单元格值。 |
| [getValues()](#getValues--) | 获取此区域中的单元格值。 |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | 指示这是否是一个区域。 |
| [isExternalLink()](#isExternalLink--) | 指示这是否是外部链接。 |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


区域的结束列。

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


区域的结束行。

**Returns:**
int
### getExternalFileName() {#getExternalFileName--}
```
public String getExternalFileName()
```


this.KeepedRels = source.KeepedRels;

**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


指示所在的工作表

**Returns:**
java.lang.String
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


区域的起始列。

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


区域的起始行。

**Returns:**
int
### getValue(int rowOffset, int colOffset) {#getValue-int-int-}
```
public Object getValue(int rowOffset, int colOffset)
```


获取相对于此区域左上角给定偏移量的单元格值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | int | 相对于此区域起始行的行偏移量 |
| colOffset | int | 列偏移量（相对于此区域的起始行） |

**Returns:**
java.lang.Object - 如果此区域无效，则返回 "\\#REF!"；如果给定的偏移超出此区域，则返回 "\\#N/A"；否则返回给定位置的单元格值。
### getValues() {#getValues--}
```
public Object getValues()
```


获取此区域中的单元格值。

**Returns:**
java.lang.Object - 如果此区域无效，将返回 \"\\#REF!\"；如果此区域是单个单元格，则返回该单元格的值对象；否则返回一个包含该区域所有值的数组。
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArea() {#isArea--}
```
public boolean isArea()
```


指示这是否是一个区域。

**Remarks**

如果这不是一个区域，则仅 StartRow 和 StartColumn 生效。

**Returns:**
boolean
### isExternalLink() {#isExternalLink--}
```
public boolean isExternalLink()
```


指示这是否是外部链接。

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

