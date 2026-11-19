---
title: "MultipleFilterCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示多个过滤器的集合。"
type: docs
url: /zh/java/com.aspose.cells/multiplefiltercollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class MultipleFilterCollection implements Iterable
```

表示多个过滤器的集合。

**Remarks**

注意：此类现已过时。请改用 [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) 。此属性将在自 2026 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [MultipleFilterCollection()](#MultipleFilterCollection--) | 构造一个新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | 添加日期过滤条件值。 |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | 添加日期时间过滤条件值。 |
| [add(String filter)](#add-java.lang.String-) | 添加标签过滤条件。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取 [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) 或字符串值。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取过滤值的计数。 |
| [getMatchBlank()](#getMatchBlank--) | 指示是否按空白进行过滤。 |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | 获取过滤值的枚举器， |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | 指示是否按空白进行过滤。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MultipleFilterCollection() {#MultipleFilterCollection--}
```
public MultipleFilterCollection()
```


构造一个新实例。

**Remarks**

注意：此成员现已过时。请改为将 FilterColumn.FilterType 设置为 FilterType.MultipleFilters，然后获取 FilterColumn.MultipleFilters。此属性将在自 2026 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

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

### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


添加标签过滤条件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 过滤器 | java.lang.String | 过滤器数据。 |

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
public Object get(int index)
```


获取 [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) 或字符串值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
java.lang.Object - 
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


获取过滤值的计数。

**Returns:**
int
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
### iterator() {#iterator--}
```
public Iterator iterator()
```


获取过滤值的枚举器，

**Returns:**
java.util.Iterator -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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

