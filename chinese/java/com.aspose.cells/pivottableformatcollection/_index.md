---
title: "PivotTableFormatCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示应用于 PivotTable 的格式集合。"
type: docs
url: /zh/java/com.aspose.cells/pivottableformatcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableFormatCollection extends CollectionBase
```

表示应用于 PivotTable 的格式集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add()](#add--) | 添加一个 [PivotTableFormat](../../com.aspose.cells/pivottableformat)。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | 格式化数据透视表的选定区域。 |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | 格式化数据透视表的选定区域。 |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | 格式化数据透视表区域中的单元格 |
| [formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style)](#formatArea-int-int-int-int-boolean-boolean-com.aspose.cells.Style-) | 格式化选定的区域。 |
| [get(int index)](#get-int-) | 根据索引获取格式。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的项。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


添加一个 [PivotTableFormat](../../com.aspose.cells/pivottableformat)。

**Returns:**
int - 新格式的索引。
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


向 CollectionBase 实例添加一个项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 要添加到 CollectionBase 实例的对象。 |

**Returns:**
int - 新元素插入的位置。
### clear() {#clear--}
```
public void clear()
```


从 CollectionBase 实例中移除所有对象。

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


返回实例是否包含此对象

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 测试对象 |

**Returns:**
boolean - 实例是否包含此对象
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
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


格式化数据透视表的选定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 单元格的范围。 |
| style | [Style](../../com.aspose.cells/style) | 样式 |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


格式化数据透视表的选定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | 选定的透视视图区域。 |
| style | [Style](../../com.aspose.cells/style) | 已格式化的设置。 |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


格式化数据透视表区域中的单元格

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 单元格的行索引 |
| 列 | int | 单元格的列索引 |
| style | [Style](../../com.aspose.cells/style) | 用于格式化单元格的样式 |

### formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style) {#formatArea-int-int-int-int-boolean-boolean-com.aspose.cells.Style-}
```
public PivotTableFormat formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style)
```


格式化选定的区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。此规则适用于 PivotTable 的区域。 |
| fieldPosition | int | 此规则适用的轴内字段的位置。 |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)。透视字段的汇总过滤类型。 |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype)。指示如何选择数据。 |
| isGrandRow | boolean | 指示是否选择总计行。 |
| isGrandColumn | boolean | 指示是否选择总计列。 |
| style | [Style](../../com.aspose.cells/style) | 应用于透视表区域的样式。 |

**Returns:**
[PivotTableFormat](../../com.aspose.cells/pivottableformat) - 
### get(int index) {#get-int-}
```
public PivotTableFormat get(int index)
```


根据索引获取格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |

**Returns:**
[PivotTableFormat](../../com.aspose.cells/pivottableformat) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


获取 CollectionBase 实例中包含的元素数量。

**Returns:**
int - CollectionBase 实例中包含的元素数量。
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


确定 CollectionBase 实例中特定项的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 确定 CollectionBase 实例中特定项的索引。 |

**Returns:**
int - 如果在列表中找到该值则返回其索引；否则返回 -1。
### iterator() {#iterator--}
```
public Iterator iterator()
```


返回遍历 CollectionBase 实例的枚举器。

**Returns:**
java.util.Iterator - 用于遍历 CollectionBase 实例的迭代器。
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


移除指定索引处的项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要移除的项的零基索引。 |

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

