---
title: "TrendlineCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示指定数据系列的所有对象的集合。"
type: docs
url: /zh/java/com.aspose.cells/trendlinecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TrendlineCollection extends CollectionBase
```

表示指定数据系列的所有 [Trendline](../../com.aspose.cells/trendline) 对象的集合。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         worksheet.getCells().get("A1").putValue(50);
         worksheet.getCells().get("A2").putValue(100);
         worksheet.getCells().get("A3").putValue(150);
         worksheet.getCells().get("A4").putValue(200);
         worksheet.getCells().get("B1").putValue(60);
         worksheet.getCells().get("B2").putValue(32);
         worksheet.getCells().get("B3").putValue(50);
         worksheet.getCells().get("B4").putValue(40);
 
         //Adding a chart to the worksheet
         int chartIndex = workbook.getWorksheets().get(0).getCharts().add(ChartType.COLUMN, 3, 3, 15, 10);
         Chart chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
         chart.getNSeries().add("A1:a3", true);
         chart.getNSeries().get(0).getTrendLines().add(TrendlineType.LINEAR, "MyTrendLine");
         Trendline line = chart.getNSeries().get(0).getTrendLines().get(0);
         line.setDisplayEquation(true);
         line.setDisplayRSquared(true);
         line.setColor(Color.getRed());
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int type)](#add-int-) | 向此集合添加具有指定类型的 [Trendline](../../com.aspose.cells/trendline) 对象。 |
| [add(int type, String name)](#add-int-java.lang.String-) | 向此集合添加具有指定类型和名称的 [Trendline](../../com.aspose.cells/trendline) 对象。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 通过索引获取 [Trendline](../../com.aspose.cells/trendline) 对象。 |
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


向此集合添加具有指定类型的 [Trendline](../../com.aspose.cells/trendline) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [TrendlineType](../../com.aspose.cells/trendlinetype)。趋势线类型。 |

**Returns:**
int - [Trendline](../../com.aspose.cells/trendline) 对象索引。
### add(int type, String name) {#add-int-java.lang.String-}
```
public int add(int type, String name)
```


向此集合添加具有指定类型和名称的 [Trendline](../../com.aspose.cells/trendline) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [TrendlineType](../../com.aspose.cells/trendlinetype)。趋势线类型。 |
| 名称 | java.lang.String | 趋势线名称。 |

**Returns:**
int - [Trendline](../../com.aspose.cells/trendline) 对象索引。
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
### get(int index) {#get-int-}
```
public Trendline get(int index)
```


通过索引获取 [Trendline](../../com.aspose.cells/trendline) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
[Trendline](../../com.aspose.cells/trendline)
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

