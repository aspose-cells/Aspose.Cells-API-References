---
title: "GridNameCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.gridweb/gridnamecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridNameCollection
```

封装一个由 [GridName](../../com.aspose.gridweb/gridname) 对象组成的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int sheetIndex, String text, String refersTo)](#add-int-java.lang.String-java.lang.String-) | 在指定的工作表中定义一个新名称。 |
| [add(String text, String refersTo)](#add-java.lang.String-java.lang.String-) | 定义一个新的全局名称。 |
| [clear()](#clear--) | 移除所有名称； |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [GridName](../../com.aspose.gridweb/gridname) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取枚举器的大小 |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | 获取行枚举器 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String[] names)](#remove-java.lang.String---) | 删除一组名称。 |
| [removeAt(int index)](#removeAt-int-) | 删除特定索引处的名称。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int sheetIndex, String text, String refersTo) {#add-int-java.lang.String-java.lang.String-}
```
public int add(int sheetIndex, String text, String refersTo)
```


在指定的工作表中定义一个新名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | int | 名称所在的工作表索引。 |
| 文本 | java.lang.String | 名称文本。它不能包含工作表名称。 |
| refersTo | java.lang.String | 名称所定义引用的公式。它必须包含工作表名称。例如：'sheet hello!'A1:B2。 |

**Returns:**
int - 名称对象索引。
### add(String text, String refersTo) {#add-java.lang.String-java.lang.String-}
```
public int add(String text, String refersTo)
```


定义一个新的全局名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文本 | java.lang.String | 名称文本。它可以包含工作表名称。 |
| refersTo | java.lang.String | 名称所定义引用的公式。它必须包含工作表名称。例如：'sheet hello!'A1:B2。 |

**Returns:**
int - 名称对象索引。
### clear() {#clear--}
```
public void clear()
```


移除所有名称；

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
public GridName get(int index)
```


获取指定索引处的 [GridName](../../com.aspose.gridweb/gridname) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[GridName](../../com.aspose.gridweb/gridname) - The element at the specified index.
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

请确保在调用方法之前，该名称未被其他公式引用。如果该名称已被引用，请仅将 Name.RefersTo 设置为 null。

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

