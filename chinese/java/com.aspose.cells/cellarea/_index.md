---
title: "CellArea"
second_title: "Aspose.Cells for Java API 参考"
description: "表示一块单元格区域。"
type: docs
url: /zh/java/com.aspose.cells/cellarea/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public final class CellArea implements Comparable
```

表示一块单元格区域。

**Example**

```
         //Create Cell Area
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CellArea()](#CellArea--) |  |
## 字段

| 字段 | 描述 |
| --- | --- |
| [EndColumn](#EndColumn) | 获取或设置此区域的结束列。 |
| [EndRow](#EndRow) | 获取或设置此区域的结束行。 |
| [StartColumn](#StartColumn) | 获取或设置此区域的起始列。 |
| [StartRow](#StartRow) | 获取或设置此区域的起始行。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [compareTo(Object obj)](#compareTo-java.lang.Object-) | 根据左上角比较两个 CellArea 对象。 |
| [createCellArea(int startRow, int startColumn, int endRow, int endColumn)](#createCellArea-int-int-int-int-) | 创建一个单元格区域。 |
| [createCellArea(String startCellName, String endCellName)](#createCellArea-java.lang.String-java.lang.String-) | 创建一个单元格区域。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | 返回表示当前单元格区域对象的字符串。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellArea() {#CellArea--}
```
public CellArea()
```


### EndColumn {#EndColumn}
```
public int EndColumn
```


获取或设置此区域的结束列。

### EndRow {#EndRow}
```
public int EndRow
```


获取或设置此区域的结束行。

### StartColumn {#StartColumn}
```
public int StartColumn
```


获取或设置此区域的起始列。

### StartRow {#StartRow}
```
public int StartRow
```


获取或设置此区域的起始行。

### compareTo(Object obj) {#compareTo-java.lang.Object-}
```
public int compareTo(Object obj)
```


根据左上角比较两个 CellArea 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
int - 如果两个角位于不同行，则比较它们的行索引。否则比较它们的列索引。如果两个角相同，则返回 0。
### createCellArea(int startRow, int startColumn, int endRow, int endColumn) {#createCellArea-int-int-int-int-}
```
public static CellArea createCellArea(int startRow, int startColumn, int endRow, int endColumn)
```


创建一个单元格区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行。 |
| startColumn | int | 起始列。 |
| endRow | int | 结束行。 |
| endColumn | int | 结束列。 |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
### createCellArea(String startCellName, String endCellName) {#createCellArea-java.lang.String-java.lang.String-}
```
public static CellArea createCellArea(String startCellName, String endCellName)
```


创建一个单元格区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startCellName | java.lang.String | 范围的左上单元格。 |
| endCellName | java.lang.String | 范围的右下单元格。 |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
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


返回表示当前单元格区域对象的字符串。

**Returns:**
java.lang.String -
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

