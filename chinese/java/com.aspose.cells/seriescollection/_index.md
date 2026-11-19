---
title: "SeriesCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.cells/seriescollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SeriesCollection extends CollectionBase
```

封装一组 [Series](../../com.aspose.cells/series) 对象。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [add(String dataArea, boolean isVertical)](#add-java.lang.String-boolean-) | 将 [Series](../../com.aspose.cells/series) 集合添加到图表中。 |
| [add(String area, boolean isVertical, boolean checkLabels)](#add-java.lang.String-boolean-boolean-) | 将 [Series](../../com.aspose.cells/series) 集合添加到图表中。 |
| [addR1C1(String area, boolean isVertical)](#addR1C1-java.lang.String-boolean-) | 将 [Series](../../com.aspose.cells/series) 集合添加到图表中。 |
| [changeColors(int type)](#changeColors-int-) | 为图表系列设置单色调色板。 |
| [changeSeriesOrder(int sourceIndex, int destIndex)](#changeSeriesOrder-int-int-) | 直接更改两个系列的顺序。 |
| [clear()](#clear--) | 清空集合 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [Series](../../com.aspose.cells/series) 元素。 |
| [getCategoryData()](#getCategoryData--) | 获取类别轴值的范围。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [getSecondCategoryData()](#getSecondCategoryData--) | 获取第二类别轴值的范围。 |
| [getSeriesByOrder(int order)](#getSeriesByOrder-int-) | 按顺序获取 [Series](../../com.aspose.cells/series) 元素。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [isColorVaried()](#isColorVaried--) | 表示点的颜色是否多样化。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 在特定索引处删除系列。 |
| [setCategoryData(String value)](#setCategoryData-java.lang.String-) | 设置类别轴值的范围。 |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | 表示点的颜色是否多样化。 |
| [setSecondCategoryData(String value)](#setSecondCategoryData-java.lang.String-) | 设置第二类别轴值的范围。 |
| [setSeriesNames(int startIndex, String area, boolean isVertical)](#setSeriesNames-int-java.lang.String-boolean-) | 设置图表中所有系列的名称。 |
| [swapSeries(int sourceIndex, int destIndex)](#swapSeries-int-int-) | 直接更改两个系列的顺序。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### add(String dataArea, boolean isVertical) {#add-java.lang.String-boolean-}
```
public int add(String dataArea, boolean isVertical)
```


将 [Series](../../com.aspose.cells/series) 集合添加到图表中。

**Remarks**


如果在连续单元格上设置数据，请使用冒号分隔。例如，$C$2:$C$5。

如果在非连续单元格上设置数据，请使用逗号分隔。例如：($C$2,$D$5)。

此方法仅简单地将其处理为数据范围。如果您想智能地检查 ChartCollection.Add() 方法。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dataArea | java.lang.String | 指定用于绘制数据系列的值 |
| isVertical | boolean | 指定是按行还是按列从单元格值范围绘制系列。如果为 true，[Series](../../com.aspose.cells/series) 将按列逐个添加。 |

**Returns:**
int - 返回在 NSeries 中添加的 ASeries 的第一个索引。
### add(String area, boolean isVertical, boolean checkLabels) {#add-java.lang.String-boolean-boolean-}
```
public int add(String area, boolean isVertical, boolean checkLabels)
```


将 [Series](../../com.aspose.cells/series) 集合添加到图表中。

**Remarks**


如果在连续单元格上设置数据，请使用冒号分隔。例如，$C$2:$C$5。

如果在非连续单元格上设置数据，请使用逗号分隔。例如，($C$2,$D$5)。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| area | java.lang.String | 指定用于绘制数据系列的值 |
| isVertical | boolean | 指定是按行还是按列从单元格值范围绘制系列。 |
| checkLabels | boolean | 指示该范围是否包含系列的名称 |

**Returns:**
int - 返回在 NSeries 中添加的 ASeries 的第一个索引。
### addR1C1(String area, boolean isVertical) {#addR1C1-java.lang.String-boolean-}
```
public int addR1C1(String area, boolean isVertical)
```


将 [Series](../../com.aspose.cells/series) 集合添加到图表中。

**Remarks**


如果在连续单元格上设置数据，请使用冒号分隔。例如，R[1]C[1]:R[3]C[2]。

如果在连续单元格上设置数据，请使用逗号分隔。例如，(R[1]C[1],R[3]C[2])。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| area | java.lang.String | 指定用于绘制数据系列的值 |
| isVertical | boolean | 指定是按行还是按列从单元格值范围绘制系列。 |

**Returns:**
int - 返回在 NSeries 中添加的 ASeries 的第一个索引。
### changeColors(int type) {#changeColors-int-}
```
public void changeColors(int type)
```


为图表系列设置单色调色板。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ChartColorPaletteType](../../com.aspose.cells/chartcolorpalettetype)。单色类型。 |

### changeSeriesOrder(int sourceIndex, int destIndex) {#changeSeriesOrder-int-int-}
```
public void changeSeriesOrder(int sourceIndex, int destIndex)
```


直接更改两个系列的顺序。

**Remarks**

注意：此方法现已过时。请改用 SeriesCollection.SwapSeries 方法。该方法将在自 2024 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceIndex | int | 当前索引 |
| destIndex | int | 目标索引 |

### clear() {#clear--}
```
public void clear()
```


清空集合

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
public Series get(int index)
```


获取指定索引处的 [Series](../../com.aspose.cells/series) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[Series](../../com.aspose.cells/series) - The element at the specified index.
### getCategoryData() {#getCategoryData--}
```
public String getCategoryData()
```


获取类别轴值的范围。它可以是单元格范围（例如 "d1:e10"）或值序列（例如 "\{2,6,8,10\}"）。

**Returns:**
java.lang.String
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
### getSecondCategoryData() {#getSecondCategoryData--}
```
public String getSecondCategoryData()
```


获取第二类别轴值的范围。它可以是单元格范围（例如 "d1:e10"），或值序列（例如 "\{2,6,8,10\}"）。仅在某些系列绘制在第二坐标轴时生效。

**Returns:**
java.lang.String
### getSeriesByOrder(int order) {#getSeriesByOrder-int-}
```
public Series getSeriesByOrder(int order)
```


按顺序获取 [Series](../../com.aspose.cells/series) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| order | int | 系列的顺序 |

**Returns:**
[Series](../../com.aspose.cells/series) - The element series
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
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


表示点的颜色是否多样化。

**Remarks**

仅在饼图或只有一个系列时有效。

**Returns:**
boolean
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


在特定索引处删除系列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |

### setCategoryData(String value) {#setCategoryData-java.lang.String-}
```
public void setCategoryData(String value)
```


设置类别轴值的范围。它可以是单元格范围（例如 \"d1:e10\"）或值序列（例如 \"\\{2,6,8,10\\}\"）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


表示点的颜色是否多样化。

**Remarks**

仅在饼图或只有一个系列时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSecondCategoryData(String value) {#setSecondCategoryData-java.lang.String-}
```
public void setSecondCategoryData(String value)
```


设置第二类别轴值的范围。它可以是单元格范围（例如 \"d1:e10\"），或值序列（例如 \"\\{2,6,8,10\\}\"）。仅在某些系列绘制在第二坐标轴时生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSeriesNames(int startIndex, String area, boolean isVertical) {#setSeriesNames-int-java.lang.String-boolean-}
```
public void setSeriesNames(int startIndex, String area, boolean isVertical)
```


设置图表中所有系列的名称。

**Remarks**


如果起始索引大于系列的计数，它将返回且不执行任何操作。

如果在连续单元格上设置数据，请使用冒号分隔。例如，$C$2:$C$5。

如果在连续单元格上设置数据，请使用逗号分隔它们。例如，($C$2,$D$5)。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startIndex | int | 您想设置名称的第一个系列的索引。 |
| area | java.lang.String | 指定系列名称的区域。 |
| isVertical | boolean | >指定是按行还是按列从单元格值范围绘制系列。 |

### swapSeries(int sourceIndex, int destIndex) {#swapSeries-int-int-}
```
public void swapSeries(int sourceIndex, int destIndex)
```


直接更改两个系列的顺序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceIndex | int | 当前索引 |
| destIndex | int | 目标索引 |

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

