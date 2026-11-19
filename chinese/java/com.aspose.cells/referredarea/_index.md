---
title: "ReferredArea"
second_title: "Aspose.Cells for Java API 参考"
description: "表示公式引用的区域。"
type: docs
url: /zh/java/com.aspose.cells/referredarea/
---

**Inheritance:**
java.lang.Object
```
public class ReferredArea
```

表示公式引用的区域。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | 区域的结束列。 |
| [getEndRow()](#getEndRow--) | 区域的结束行。 |
| [getExternalFileName()](#getExternalFileName--) | 如果这是外部引用，则获取外部文件名。 |
| [getSheetName()](#getSheetName--) | 指示此引用所在的工作表。 |
| [getSheetNames()](#getSheetNames--) | 此实例引用的所有工作表的名称。 |
| [getStartColumn()](#getStartColumn--) | 区域的起始列。 |
| [getStartRow()](#getStartRow--) | 区域的起始行。 |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | 获取相对于此区域左上角给定偏移量的单元格值。 |
| [getValue(int rowOffset, int colOffset, boolean calculateFormulas)](#getValue-int-int-boolean-) | 获取相对于此区域左上角给定偏移量的单元格值。 |
| [getValues()](#getValues--) | 获取此区域中的单元格值。 |
| [getValues(boolean calculateFormulas)](#getValues-boolean-) | 获取此区域中的单元格值。 |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | 指示这是否是一个区域。 |
| [isEntireColumn()](#isEntireColumn--) | 指示此区域是否包含所有行（整列）。 |
| [isEntireRow()](#isEntireRow--) | 指示此区域是否包含所有列（整行）。 |
| [isExternalLink()](#isExternalLink--) | 指示这是否是外部链接。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | 返回此区域的引用地址。 |
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


如果这是外部引用，则获取外部文件名。

**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


指示此引用所在的工作表。

**Remarks**

如果它引用多个工作表，返回的值类似于公式中的范围表达式。例如，对于公式 "=SUM(Sheet1:Sheet3!$A$1:$B$2)" 中的引用，返回值为 "Sheet1:Sheet3"。

**Returns:**
java.lang.String
### getSheetNames() {#getSheetNames--}
```
public String[] getSheetNames()
```


此实例引用的所有工作表的名称。

**Returns:**
java.lang.String[]
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
### getValue(int rowOffset, int colOffset, boolean calculateFormulas) {#getValue-int-int-boolean-}
```
public Object getValue(int rowOffset, int colOffset, boolean calculateFormulas)
```


获取相对于此区域左上角给定偏移量的单元格值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | int | 相对于此区域起始行的行偏移量 |
| colOffset | int | 列偏移量（相对于此区域的起始行） |
| calculateFormulas | boolean | 如果指定的引用是公式，是否递归计算它 |

**Returns:**
java.lang.Object - 如果此区域无效，则返回 "\\#REF!"；如果给定的偏移超出此区域，则返回 "\\#N/A"；否则返回给定位置的单元格值。
### getValues() {#getValues--}
```
public Object getValues()
```


获取此区域中的单元格值。

**Returns:**
java.lang.Object - 如果此区域无效，将返回 "\\#REF!"；如果此区域是单个单元格，则返回该单元格的值对象；否则返回一个包含此区域所有值的二维数组。
### getValues(boolean calculateFormulas) {#getValues-boolean-}
```
public Object getValues(boolean calculateFormulas)
```


获取此区域中的单元格值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| calculateFormulas | boolean | 在此范围内，如果存在尚未计算的公式，此标志指示是否应递归计算这些公式 |

**Returns:**
java.lang.Object - 如果此区域无效，将返回 "\\#REF!"；如果此区域是单个单元格，则返回该单元格的值对象；否则返回一个包含此区域所有值的二维数组。
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
### isEntireColumn() {#isEntireColumn--}
```
public boolean isEntireColumn()
```


指示此区域是否包含所有行（整列）。

**Returns:**
boolean
### isEntireRow() {#isEntireRow--}
```
public boolean isEntireRow()
```


指示此区域是否包含所有列（整行）。

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


返回此区域的引用地址。通常它是可在公式中使用的引用地址，例如 "Sheet1!A1:C3"。

**Returns:**
java.lang.String - 此区域的引用地址。
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

