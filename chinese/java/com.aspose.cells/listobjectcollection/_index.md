---
title: "ListObjectCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作表中对象的集合。"
type: docs
url: /zh/java/com.aspose.cells/listobjectcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ListObjectCollection extends CollectionBase
```

表示工作表中 [ListObject](../../com.aspose.cells/listobject) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#add-int-int-int-int-boolean-) | 向工作表添加 ListObject。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [add(String startCell, String endCell, boolean hasHeaders)](#add-java.lang.String-java.lang.String-boolean-) | 向工作表添加 ListObject。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 通过索引获取 ListObject。 |
| [get(String tableName)](#get-java.lang.String-) | 通过指定名称获取 ListObject。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 通过索引移除 [ListObject](../../com.aspose.cells/listobject)。 |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | 更新表的所有列名。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#add-int-int-int-int-boolean-}
```
public int add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


向工作表添加 ListObject。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 列表范围的起始行。 |
| startColumn | int | 列表范围的起始行。 |
| endRow | int | 列表范围的起始行。 |
| endColumn | int | 列表范围的起始行。 |
| hasHeaders | boolean | 范围是否具有标题。 |

**Returns:**
int - 新 ListObject 的索引
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
### add(String startCell, String endCell, boolean hasHeaders) {#add-java.lang.String-java.lang.String-boolean-}
```
public int add(String startCell, String endCell, boolean hasHeaders)
```


向工作表添加 ListObject。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startCell | java.lang.String | 列表范围的起始单元格。 |
| endCell | java.lang.String | 列表范围的结束单元格。 |
| hasHeaders | boolean | 范围是否具有标题。 |

**Returns:**
int - 新 ListObject 的索引
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
public ListObject get(int index)
```


通过索引获取 ListObject。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - The ListObject
### get(String tableName) {#get-java.lang.String-}
```
public ListObject get(String tableName)
```


通过指定名称获取 ListObject。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tableName | java.lang.String | ListObject 名称。 |

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - The ListObject
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


通过索引移除 [ListObject](../../com.aspose.cells/listobject)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


更新表的所有列名。

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

