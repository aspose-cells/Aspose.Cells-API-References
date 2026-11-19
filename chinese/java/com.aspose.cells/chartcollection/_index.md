---
title: "ChartCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.cells/chartcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ChartCollection extends CollectionBase
```

封装一个包含 [Chart](../../com.aspose.cells/chart) 对象的集合。

**Example**

```
         Workbook workbook = new Workbook();
 
         ChartCollection charts = workbook.getWorksheets().get(0).getCharts();
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-byte---java.lang.String-boolean-int-int-int-int-) | 添加一个带有预设模板的图表。 |
| [add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)](#add-int-int-int-int-int-) | 向集合中添加图表。 |
| [add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-boolean-int-int-int-int-) | 向集合中添加图表。 |
| [add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-int-int-int-int-) | 向集合中添加图表。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [addFloatingChart(int type, int left, int top, int width, int height)](#addFloatingChart-int-int-int-int-int-) | 向集合中添加图表。 |
| [clear()](#clear--) | 清除所有图表。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [Chart](../../com.aspose.cells/chart) 元素。 |
| [get(String name)](#get-java.lang.String-) | 按名称获取图表。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Chart chart)](#remove-com.aspose.cells.Chart-) | 移除指定的图表。 |
| [removeAt(int index)](#removeAt-int-) | 在指定索引处移除图表。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-byte---java.lang.String-boolean-int-int-int-int-}
```
public int add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


添加一个带有预设模板的图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 数据 | byte[] | 图表模板文件（.crtx）的数据。 |
| dataRange | java.lang.String | 指定图表的数据范围 |
| isVertical | boolean | 指定是按行还是按列从单元格值范围绘制系列。 |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| rightRow | int | 右下行索引 |
| bottomColumn | int | 右下列索引 |

**Returns:**
int - [Chart](../../com.aspose.cells/chart) 对象索引。
### add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn) {#add-int-int-int-int-int-}
```
public int add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```


向集合中添加图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype)。图表类型 |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| bottomRow | int | 右下行索引 |
| rightColumn | int | 右下列索引 |

**Returns:**
int - [Chart](../../com.aspose.cells/chart) 对象索引。
### add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-boolean-int-int-int-int-}
```
public int add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


向集合中添加图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype)。图表类型 |
| dataRange | java.lang.String | 指定图表的数据范围 |
| isVertical | boolean | 指定是按行还是按列从单元格值范围绘制系列。 |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| rightRow | int | 右下行索引 |
| bottomColumn | int | 右下列索引 |

**Returns:**
int - [Chart](../../com.aspose.cells/chart) 对象索引。
### add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-int-int-int-int-}
```
public int add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


向集合中添加图表。

**Remarks**

注意：此成员已过时。请改用 [add(int,String,boolean,int,int,int,int)](../../com.aspose.cells/chartcollection\#add-int-String-boolean-int-int-int-int-) 属性。该属性将在自2022年5月起的12个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype)。图表类型 |
| dataRange | java.lang.String | 指定图表的数据范围 |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| rightRow | int | 右下行索引 |
| bottomColumn | int | 右下列索引 |

**Returns:**
int - [Chart](../../com.aspose.cells/chart) 对象索引。
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
### addFloatingChart(int type, int left, int top, int width, int height) {#addFloatingChart-int-int-int-int-int-}
```
public int addFloatingChart(int type, int left, int top, int width, int height)
```


向集合中添加图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype)。图表类型 |
| 左侧 | int | 到角落的 x 偏移量 |
| 顶部 | int | 到角落的 y 偏移量 |
| 宽度 | int | 图表宽度 |
| 高度 | int | 图表高度 |

**Returns:**
int - [Chart](../../com.aspose.cells/chart) 对象索引。
### clear() {#clear--}
```
public void clear()
```


清除所有图表。

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
public Chart get(int index)
```


获取指定索引处的 [Chart](../../com.aspose.cells/chart) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public Chart get(String name)
```


按名称获取图表。

**Remarks**

默认的图表名称为 null。因此您必须显式设置图表的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 图表名称。 |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The chart.
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




### remove(Chart chart) {#remove-com.aspose.cells.Chart-}
```
public void remove(Chart chart)
```


移除指定的图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| chart | [Chart](../../com.aspose.cells/chart) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


在指定索引处移除图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 图表索引。 |

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

