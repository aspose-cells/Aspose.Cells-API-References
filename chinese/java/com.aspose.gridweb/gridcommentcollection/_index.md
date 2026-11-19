---
title: "GridCommentCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.gridweb/gridcommentcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridCommentCollection
```

封装一个 [GridComment](../../com.aspose.gridweb/gridcomment) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | 向集合添加评论。 |
| [add(String cellName)](#add-java.lang.String-) | 向集合添加评论。 |
| [clear()](#clear--) | 移除所有评论； |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [GridComment](../../com.aspose.gridweb/gridcomment) 元素。 |
| [get(int row, int column)](#get-int-int-) | 获取指定行索引和列索引处的 [GridComment](../../com.aspose.gridweb/gridcomment) 元素。 |
| [get(String cellName)](#get-java.lang.String-) | 获取指定单元格处的 [GridComment](../../com.aspose.gridweb/gridcomment) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取枚举器的大小 |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | 获取行枚举器 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int row, int column)](#removeAt-int-int-) | 移除特定单元格的评论。 |
| [removeAt(String cellName)](#removeAt-java.lang.String-) | 移除特定单元格的评论。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


向集合添加评论。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 单元格行索引。 |
| 列 | int | 单元格列索引。 |

**Returns:**
int - [GridComment](../../com.aspose.gridweb/gridcomment) 对象索引。
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


向集合添加评论。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称。 |

**Returns:**
int - [GridComment](../../com.aspose.gridweb/gridcomment) 对象索引。
### clear() {#clear--}
```
public void clear()
```


移除所有评论；

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
public GridComment get(int index)
```


获取指定索引处的 [GridComment](../../com.aspose.gridweb/gridcomment) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified index.
### get(int row, int column) {#get-int-int-}
```
public GridComment get(int row, int column)
```


获取指定行索引和列索引处的 [GridComment](../../com.aspose.gridweb/gridcomment) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified cell.
### get(String cellName) {#get-java.lang.String-}
```
public GridComment get(String cellName)
```


获取指定单元格处的 [GridComment](../../com.aspose.gridweb/gridcomment) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称。 |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified cell.
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


获取枚举器的大小

**Returns:**
int
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


获取行枚举器

**Returns:**
java.util.Iterator - 行枚举器
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int row, int column) {#removeAt-int-int-}
```
public void removeAt(int row, int column)
```


移除特定单元格的评论。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

### removeAt(String cellName) {#removeAt-java.lang.String-}
```
public void removeAt(String cellName)
```


移除特定单元格的评论。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 包含注释的单元格名称。 |

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

