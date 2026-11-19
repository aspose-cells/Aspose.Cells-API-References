---
title: "PivotFieldCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示数据透视表不同区域中所有 PivotField 对象的集合。"
type: docs
url: /zh/java/com.aspose.cells/pivotfieldcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFieldCollection extends CollectionBase
```

表示数据透视表不同区域中所有 PivotField 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(PivotField pivotField)](#add-com.aspose.cells.PivotField-) | 向特定类型的 PivotFields 添加 PivotField 对象。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [addByBaseIndex(int baseFieldIndex)](#addByBaseIndex-int-) | 向特定类型的 PivotFields 添加 PivotField 对象。 |
| [clear()](#clear--) | 清除 PivotFieldCollection 的所有字段 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取特定索引处的 PivotField 对象。 |
| [get(String name)](#get-java.lang.String-) | 获取特定名称的 PivotField 对象。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [getType()](#getType--) | 获取 PivotFields 类型。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [insert(int index, PivotField pivotField)](#insert-int-com.aspose.cells.PivotField-) | 在特定索引处插入 PivotField。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [move(int currPos, int destPos)](#move-int-int-) | 将 PivotField 从当前位置移动到目标位置 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotField pivotField)](#remove-com.aspose.cells.PivotField-) | 从当前区域删除字段。 |
| [removeAt(int index)](#removeAt-int-) | 通过索引删除字段。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotField pivotField) {#add-com.aspose.cells.PivotField-}
```
public int add(PivotField pivotField)
```


向特定类型的 PivotFields 添加 PivotField 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | 一个 PivotField 对象。 |

**Returns:**
int - 此 PivotFields 中 PivotField 对象的索引。
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
### addByBaseIndex(int baseFieldIndex) {#addByBaseIndex-int-}
```
public int addByBaseIndex(int baseFieldIndex)
```


向特定类型的 PivotFields 添加 PivotField 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| baseFieldIndex | int | 基准 PivotFields 中的字段索引。 |

**Returns:**
int - 此 PivotFields 中 PivotField 对象的索引。
### clear() {#clear--}
```
public void clear()
```


清除 PivotFieldCollection 的所有字段

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
public PivotField get(int index)
```


获取特定索引处的 PivotField 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### get(String name) {#get-java.lang.String-}
```
public PivotField get(String name)
```


获取特定名称的 PivotField 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
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
### getType() {#getType--}
```
public int getType()
```


获取 PivotFields 类型。

请参阅 [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。

**Returns:**
int
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
### insert(int index, PivotField pivotField) {#insert-int-com.aspose.cells.PivotField-}
```
public void insert(int index, PivotField pivotField)
```


在特定索引处插入 PivotField。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | 该字段。 |

### iterator() {#iterator--}
```
public Iterator iterator()
```


返回遍历 CollectionBase 实例的枚举器。

**Returns:**
java.util.Iterator - 用于遍历 CollectionBase 实例的迭代器。
### move(int currPos, int destPos) {#move-int-int-}
```
public void move(int currPos, int destPos)
```


将 PivotField 从当前位置移动到目标位置

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| currPos | int | 基于零的 PivotField 当前位置 |
| destPos | int | 基于零的 PivotField 目标位置 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(PivotField pivotField) {#remove-com.aspose.cells.PivotField-}
```
public void remove(PivotField pivotField)
```


从当前区域删除字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


通过索引删除字段。仅适用于筛选、行、列、数据区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

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

