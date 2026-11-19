---
title: "FilterValueCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示多个过滤器的集合。"
type: docs
url: /zh/java/com.aspose.cells/filtervaluecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class FilterValueCollection extends CollectionBase
```

表示多个过滤器的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | 添加日期过滤条件值。 |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | 添加日期时间过滤条件值。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [add(String filter)](#add-java.lang.String-) | 添加标签过滤条件。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 通过索引获取 [FilterValue](../../com.aspose.cells/filtervalue)。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [getMatchBlank()](#getMatchBlank--) | 指示是否按空白进行过滤。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的项。 |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | 指示是否按空白进行过滤。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int type, int year, int month, int day) {#add-int-int-int-int-}
```
public void add(int type, int year, int month, int day)
```


添加日期过滤条件值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype)。日期过滤器的类型。 |
| 年 | int | 年份。 |
| 月 | int | 月份。 |
| 日 | int | 日期。 |

### add(int type, int year, int month, int day, int hour, int minute, int second) {#add-int-int-int-int-int-int-int-}
```
public void add(int type, int year, int month, int day, int hour, int minute, int second)
```


添加日期时间过滤条件值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype)。日期过滤器的类型。 |
| 年 | int | 年份。 |
| 月 | int | 月份。 |
| 日 | int | 日期。 |
| 小时 | int | 小时。 |
| 分钟 | int | 分钟。 |
| 秒 | int | 秒。 |

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
### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


添加标签过滤条件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 过滤器 | java.lang.String | 过滤器数据。 |

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
public FilterValue get(int index)
```


通过索引获取 [FilterValue](../../com.aspose.cells/filtervalue)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
[FilterValue](../../com.aspose.cells/filtervalue) - 
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
### getMatchBlank() {#getMatchBlank--}
```
public boolean getMatchBlank()
```


指示是否按空白进行过滤。

**Returns:**
boolean
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

### setMatchBlank(boolean value) {#setMatchBlank-boolean-}
```
public void setMatchBlank(boolean value)
```


指示是否按空白进行过滤。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

