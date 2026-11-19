---
title: "TableStyleElementCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示表格样式的所有元素。"
type: docs
url: /zh/java/com.aspose.cells/tablestyleelementcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TableStyleElementCollection extends CollectionBase
```

表示表格样式的所有元素。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int type)](#add-int-) | 添加一个元素。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 通过索引获取表样式的元素。 |
| [getByTableStyleElementType(int type)](#getByTableStyleElementType-int-) | 通过元素类型获取表样式的元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [getTableStyleElementWithIndex(int index)](#getTableStyleElementWithIndex-int-) | 通过索引获取表样式的元素。 |
| [getTableStyleElementWithType(int type)](#getTableStyleElementWithType-int-) | 通过元素类型获取表样式的元素。 |
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


添加一个元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [TableStyleElementType](../../com.aspose.cells/tablestyleelementtype)。元素的类型 |

**Returns:**
int - 返回列表中元素的索引。
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
public TableStyleElement get(int index)
```


通过索引获取表样式的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement) - Returns [TableStyleElement](../../com.aspose.cells/tablestyleelement) object
### getByTableStyleElementType(int type) {#getByTableStyleElementType-int-}
```
public TableStyleElement getByTableStyleElementType(int type)
```


通过元素类型获取表样式的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [TableStyleElementType](../../com.aspose.cells/tablestyleelementtype)。元素类型。 |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement) - Returns [TableStyleElement](../../com.aspose.cells/tablestyleelement) object
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
### getTableStyleElementWithIndex(int index) {#getTableStyleElementWithIndex-int-}
```
public TableStyleElement getTableStyleElementWithIndex(int index)
```


通过索引获取表样式的元素。

**Remarks**

注意：此成员已过时。请改用 Aspose.Cells.Tables.TableStyleElementCollection.this[int index] 属性。该属性将在自 2012 年 1 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement)
### getTableStyleElementWithType(int type) {#getTableStyleElementWithType-int-}
```
public TableStyleElement getTableStyleElementWithType(int type)
```


通过元素类型获取表样式的元素。

**Remarks**

注意：此成员已过时。请改用 Aspose.Cells.Tables.TableStyleElementCollection.this[TableStyleElementType type] 属性。该属性将在自 2012 年 1 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 类型 | int |  |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement)
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

