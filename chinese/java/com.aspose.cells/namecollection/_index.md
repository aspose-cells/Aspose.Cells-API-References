---
title: "NameCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示电子表格中所有对象的集合。"
type: docs
url: /zh/java/com.aspose.cells/namecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class NameCollection extends CollectionBase
```

表示电子表格中所有 [Name](../../com.aspose.cells/name) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [add(String text)](#add-java.lang.String-) | 定义一个新名称。 |
| [clear()](#clear--) | 删除所有未被公式和数据源引用的已定义名称。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int type, int sheetIndex)](#filter-int-int-) | 按作用域获取所有已定义名称。 |
| [get(int index)](#get-int-) | 获取指定索引处的 [Name](../../com.aspose.cells/name) 元素。 |
| [get(String text)](#get-java.lang.String-) | 获取具有指定名称的 [Name](../../com.aspose.cells/name) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String text)](#remove-java.lang.String-) | 删除该名称。 |
| [remove(String[] names)](#remove-java.lang.String---) | 删除一组名称。 |
| [removeAt(int index)](#removeAt-int-) | 删除特定索引处的名称。 |
| [removeDuplicateNames()](#removeDuplicateNames--) | 删除重复的已定义名称。 |
| [sort()](#sort--) | 对已定义名称进行排序。 |
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
### add(String text) {#add-java.lang.String-}
```
public int add(String text)
```


定义一个新名称。

**Remarks**

名称不能包含空格，也不能类似于单元格引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文本 | java.lang.String | 用作名称的文本。 |

**Returns:**
int - [Name](../../com.aspose.cells/name) 对象索引。
### clear() {#clear--}
```
public void clear()
```


删除所有未被公式和数据源引用的已定义名称。如果已定义名称被引用，我们仅将 Name.ReferTo 设置为 null 并隐藏它们。

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
### filter(int type, int sheetIndex) {#filter-int-int-}
```
public Name[] filter(int type, int sheetIndex)
```


按作用域获取所有已定义名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [NameScopeType](../../com.aspose.cells/namescopetype)。作用域类型。 |
| sheetIndex | int | 工作表索引。仅在作用域类型为 [NameScopeType.WORKSHEET](../../com.aspose.cells/namescopetype\#WORKSHEET) 时生效。 |

**Returns:**
com.aspose.cells.Name[] -
### get(int index) {#get-int-}
```
public Name get(int index)
```


获取指定索引处的 [Name](../../com.aspose.cells/name) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[Name](../../com.aspose.cells/name) - The element at the specified index.
### get(String text) {#get-java.lang.String-}
```
public Name get(String text)
```


获取具有指定名称的 [Name](../../com.aspose.cells/name) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文本 | java.lang.String | 名称文本。 |

**Returns:**
[Name](../../com.aspose.cells/name) - The element with the specified name.
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




### remove(String text) {#remove-java.lang.String-}
```
public void remove(String text)
```


删除该名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文本 | java.lang.String | 该名称文本。 |

### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```


删除一组名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String[] | 名称的文本。 |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


删除特定索引处的名称。

**Remarks**

请确保在调用方法之前，该名称未被其他公式引用。如果该名称已被引用，将 Name.RefersTo 设置为 null 更好。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要删除的 Name 的索引。 |

### removeDuplicateNames() {#removeDuplicateNames--}
```
public void removeDuplicateNames()
```


删除重复的已定义名称。

### sort() {#sort--}
```
public void sort()
```


对已定义名称进行排序。

**Remarks**

如果在 Excel 文件中创建了大量命名范围，请在创建完所有命名范围并在保存之前调用此方法。

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

