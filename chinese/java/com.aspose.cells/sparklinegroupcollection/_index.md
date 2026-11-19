---
title: "SparklineGroupCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.cells/sparklinegroupcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SparklineGroupCollection extends CollectionBase
```

封装一个 [SparklineGroup](../../com.aspose.cells/sparklinegroup) 对象的集合。

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
 
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, "A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         book.save("output.xlsx", SaveFormat.XLSX);
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int type)](#add-int-) | 向集合中添加一个带有 [Sparkline](../../com.aspose.cells/sparkline) 的 [SparklineGroup](../../com.aspose.cells/sparklinegroup)。 |
| [add(int type, String dataRange, boolean isVertical, CellArea locationRange)](#add-int-java.lang.String-boolean-com.aspose.cells.CellArea-) | 向集合中添加一个包含一些 [Sparkline](../../com.aspose.cells/sparkline) 的 [SparklineGroup](../../com.aspose.cells/sparklinegroup)。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [clearSparklineGroups(CellArea cellArea)](#clearSparklineGroups-com.aspose.cells.CellArea-) | 清除与单元格区域重叠的 sparkline 组。 |
| [clearSparklines(CellArea cellArea)](#clearSparklines-com.aspose.cells.CellArea-) | 清除位于单元格区域内的 sparklines。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [SparklineGroup](../../com.aspose.cells/sparklinegroup) 元素。 |
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
### add(int type) {#add-int-}
```
public int add(int type)
```


向集合中添加一个带有 [Sparkline](../../com.aspose.cells/sparkline) 的 [SparklineGroup](../../com.aspose.cells/sparklinegroup)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [SparklineType](../../com.aspose.cells/sparklinetype)。指定 Sparkline 组的类型。 |

**Returns:**
int - [SparklineGroup](../../com.aspose.cells/sparklinegroup) 对象索引。
### add(int type, String dataRange, boolean isVertical, CellArea locationRange) {#add-int-java.lang.String-boolean-com.aspose.cells.CellArea-}
```
public int add(int type, String dataRange, boolean isVertical, CellArea locationRange)
```


向集合中添加一个包含一些 [Sparkline](../../com.aspose.cells/sparkline) 的 [SparklineGroup](../../com.aspose.cells/sparklinegroup)。

**Remarks**

此方法也会创建 sparklines。如果  为 true，则 dataRange 和 locationRange 中的行数必须相同。如果  为 false，则 dataRange 和 locationRange 中的列数必须相同。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [SparklineType](../../com.aspose.cells/sparklinetype)。指定 Sparkline 组的类型。 |
| dataRange | java.lang.String | 指定 sparkline 组的数据范围。 |
| isVertical | boolean | 指定是按行还是按列从数据范围绘制 sparklines。 |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | 指定迷你图的放置位置。 |

**Returns:**
int - [SparklineGroup](../../com.aspose.cells/sparklinegroup) 对象索引。
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

### clearSparklineGroups(CellArea cellArea) {#clearSparklineGroups-com.aspose.cells.CellArea-}
```
public void clearSparklineGroups(CellArea cellArea)
```


清除与单元格区域重叠的 sparkline 组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | 指定单元格区域 |

### clearSparklines(CellArea cellArea) {#clearSparklines-com.aspose.cells.CellArea-}
```
public void clearSparklines(CellArea cellArea)
```


清除位于单元格区域内的 sparklines。

**Remarks**

[SparklineGroup](../../com.aspose.cells/sparklinegroup) will be removed too if it does not contains any [Sparkline](../../com.aspose.cells/sparkline).

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | 指定单元格区域 |

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
### get(int index) {#get-int-}
```
public SparklineGroup get(int index)
```


获取指定索引处的 [SparklineGroup](../../com.aspose.cells/sparklinegroup) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[SparklineGroup](../../com.aspose.cells/sparklinegroup) - The element at the specified index.
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

