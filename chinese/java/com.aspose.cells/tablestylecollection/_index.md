---
title: "TableStyleCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示所有自定义表格样式。"
type: docs
url: /zh/java/com.aspose.cells/tablestylecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TableStyleCollection extends CollectionBase
```

表示所有自定义表格样式。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [addPivotTableStyle(String name)](#addPivotTableStyle-java.lang.String-) | 添加自定义数据透视表样式。 |
| [addTableStyle(String name)](#addTableStyle-java.lang.String-) | 添加自定义表格样式。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 通过索引获取表格样式。 |
| [get(String name)](#get-java.lang.String-) | 通过名称获取表格样式。 |
| [getBuiltinTableStyle(int type)](#getBuiltinTableStyle-int-) | 获取内置表格样式 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [getDefaultPivotStyleName()](#getDefaultPivotStyleName--) | 获取数据透视表的默认样式名称。 |
| [getDefaultTableStyleName()](#getDefaultTableStyleName--) | 获取表格的默认样式名称。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的项。 |
| [setDefaultPivotStyleName(String value)](#setDefaultPivotStyleName-java.lang.String-) | 设置数据透视表的默认样式名称。 |
| [setDefaultTableStyleName(String value)](#setDefaultTableStyleName-java.lang.String-) | 设置表格的默认样式名称。 |
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
### addPivotTableStyle(String name) {#addPivotTableStyle-java.lang.String-}
```
public int addPivotTableStyle(String name)
```


添加自定义数据透视表样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 数据透视表样式名称。 |

**Returns:**
int - 数据透视表样式的索引。
### addTableStyle(String name) {#addTableStyle-java.lang.String-}
```
public int addTableStyle(String name)
```


添加自定义表格样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 表格样式名称。 |

**Returns:**
int - 表格样式的索引。
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
public TableStyle get(int index)
```


通过索引获取表格样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 表格样式在列表中的位置。 |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - The table style object.
### get(String name) {#get-java.lang.String-}
```
public TableStyle get(String name)
```


通过名称获取表格样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 表格样式名称。 |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - The table style object.
### getBuiltinTableStyle(int type) {#getBuiltinTableStyle-int-}
```
public TableStyle getBuiltinTableStyle(int type)
```


获取内置表格样式

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [TableStyleType](../../com.aspose.cells/tablestyletype). 内置表格样式类型。 |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - 
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
### getDefaultPivotStyleName() {#getDefaultPivotStyleName--}
```
public String getDefaultPivotStyleName()
```


获取数据透视表的默认样式名称。

**Returns:**
java.lang.String
### getDefaultTableStyleName() {#getDefaultTableStyleName--}
```
public String getDefaultTableStyleName()
```


获取表格的默认样式名称。

**Returns:**
java.lang.String
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

### setDefaultPivotStyleName(String value) {#setDefaultPivotStyleName-java.lang.String-}
```
public void setDefaultPivotStyleName(String value)
```


设置数据透视表的默认样式名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDefaultTableStyleName(String value) {#setDefaultTableStyleName-java.lang.String-}
```
public void setDefaultTableStyleName(String value)
```


设置表格的默认样式名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

