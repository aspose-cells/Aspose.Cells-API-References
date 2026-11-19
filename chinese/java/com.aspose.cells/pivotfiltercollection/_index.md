---
title: "PivotFilterCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示所有 PivotFilter 的集合。"
type: docs
url: /zh/java/com.aspose.cells/pivotfiltercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFilterCollection extends CollectionBase
```

表示所有 PivotFilter 的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int fieldIndex, int type)](#add-int-int-) | 向特定类型添加 PivotFilter 对象 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)](#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | 按行或列透视字段的日期设置进行筛选。 |
| [addLabelFilter(int baseFieldIndex, int type, String label1, String label2)](#addLabelFilter-int-int-java.lang.String-java.lang.String-) | 按行或列透视字段的标题进行筛选。 |
| [addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)](#addTop10Filter-int-int-int-boolean-int-) | 按数据透视字段的值进行筛选。 |
| [addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)](#addValueFilter-int-int-int-double-double-) | 按数据透视字段的值进行筛选。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [clearFilter(int fieldIndex)](#clearFilter-int-) | 从特定 PivotField 中清除 PivotFilter |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取特定索引处的 pivotfilter 对象。 |
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
### add(int fieldIndex, int type) {#add-int-int-}
```
public int add(int fieldIndex, int type)
```


向特定类型添加 PivotFilter 对象

**Remarks**

注意：此方法现已过时。请改用 PivotFilterCollection.AddValueFilter()、AddTop10Filter()、AddLabelFilter() 和 AddDateFilter() 方法。该方法将在自 2024 年 11 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | PivotField 的索引 |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). PivotFilter 类型 |

**Returns:**
int - 此 PivotFilterCollection 中 PivotFilter 对象的索引。
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
### addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2) {#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)
```


按行或列透视字段的日期设置进行筛选。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| baseFieldIndex | int | 源中字段的索引。 |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). 过滤数据的类型。 |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | 过滤条件的日期标签 |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | 介于过滤条件之间的上限日期标签 |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addLabelFilter(int baseFieldIndex, int type, String label1, String label2) {#addLabelFilter-int-int-java.lang.String-java.lang.String-}
```
public PivotFilter addLabelFilter(int baseFieldIndex, int type, String label1, String label2)
```


按行或列透视字段的标题进行筛选。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| baseFieldIndex | int | 源中字段的索引。 |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). 过滤数据的类型。 |
| label1 | java.lang.String | 过滤条件的标签 |
| label2 | java.lang.String | 介于过滤条件之间的上限标签 |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount) {#addTop10Filter-int-int-int-boolean-int-}
```
public PivotFilter addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)
```


按数据透视字段的值进行筛选。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| baseFieldIndex | int | 源中字段的索引。 |
| valueFieldIndex | int | 数据区域中数据字段的索引。 |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). 过滤数据的类型。仅可为 Count、Sum 和 Percent。 |
| isTop | boolean | 指示过滤是来自顶部还是底部 |
| itemCount | int | 项目计数 |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2) {#addValueFilter-int-int-int-double-double-}
```
public PivotFilter addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)
```


按数据透视字段的值进行筛选。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| baseFieldIndex | int | 源中字段的索引。 |
| valueFieldIndex | int | 值区域中值字段的索引。 |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). 过滤数据的类型。 |
| value1 | double | 过滤条件的值 |
| value2 | double | 介于过滤条件之间的上限值 |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### clear() {#clear--}
```
public void clear()
```


从 CollectionBase 实例中移除所有对象。

### clearFilter(int fieldIndex) {#clearFilter-int-}
```
public void clearFilter(int fieldIndex)
```


从特定 PivotField 中清除 PivotFilter

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | PivotField 的索引 |

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
public PivotFilter get(int index)
```


获取特定索引处的 pivotfilter 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
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

