---
title: "HorizontalPageBreakCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.cells/horizontalpagebreakcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HorizontalPageBreakCollection extends CollectionBase
```

封装一个由 [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) 对象组成的集合。

**Example**

```
         Workbook excel = new Workbook();
 
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int row)](#add-int-) | 向集合中添加水平分页符。 |
| [add(int row, int column)](#add-int-int-) | 向集合中添加水平分页符。 |
| [add(int row, int startColumn, int endColumn)](#add-int-int-int-) | 向集合中添加水平分页符。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [add(String cellName)](#add-java.lang.String-) | 向集合中添加水平分页符。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) 元素。 |
| [get(String cellName)](#get-java.lang.String-) | 获取具有指定单元格名称的 [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 移除具有指定名称的 HPageBreak 元素。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row) {#add-int-}
```
public int add(int row)
```


向集合中添加水平分页符。

**Remarks**

分页符被添加在单元格的左上角。请同时设置水平分页符和垂直分页符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 单元格行索引，零基。 |

**Returns:**
int - [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) 对象索引。
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


向集合中添加水平分页符。

**Remarks**

分页符被添加在单元格的左上角。请同时设置水平分页符和垂直分页符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 单元格行索引，零基。 |
| 列 | int | 单元格列索引，零基。 |

**Returns:**
int - [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) 对象索引。
### add(int row, int startColumn, int endColumn) {#add-int-int-int-}
```
public int add(int row, int startColumn, int endColumn)
```


向集合中添加水平分页符。

**Remarks**

此方法用于在打印区域内添加水平分页符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引，基于零。 |
| startColumn | int | 起始列索引，基于零。 |
| endColumn | int | 结束列索引，基于零。 |

**Returns:**
int - [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) 对象索引。
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
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


向集合中添加水平分页符。

**Remarks**

分页符被添加在单元格的左上角。请同时设置水平分页符和垂直分页符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称。 |

**Returns:**
int - [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) 对象索引。
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
public HorizontalPageBreak get(int index)
```


获取指定索引处的 [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public HorizontalPageBreak get(String cellName)
```


获取具有指定单元格名称的 [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称。 |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element with the specified cell name.
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


移除具有指定名称的 HPageBreak 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素索引，零基。 |

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

