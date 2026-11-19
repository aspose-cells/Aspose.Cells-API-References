---
title: "GridValidationCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.gridweb/gridvalidationcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridValidationCollection
```

封装一个 [GridValidation](../../com.aspose.gridweb/gridvalidation) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add()](#add--) | 向集合中添加一个 [GridValidation](../../com.aspose.gridweb/gridvalidation)。 |
| [add(GridCellArea ca)](#add-com.aspose.gridweb.GridCellArea-) | 向集合添加数据验证。 |
| [add(GridValidation validation)](#add-com.aspose.gridweb.GridValidation-) | 向集合中添加一个 [GridValidation](../../com.aspose.gridweb/gridvalidation)。 |
| [add(int row, int column)](#add-int-int-) | 向集合中添加一个 [GridValidation](../../com.aspose.gridweb/gridvalidation)。验证将应用于指定的单元格。 |
| [add(String cellname)](#add-java.lang.String-) | 向集合中添加一个 [GridValidation](../../com.aspose.gridweb/gridvalidation)。验证将应用于指定的单元格。 |
| [clear()](#clear--) | 清除所有验证。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [GridValidation](../../com.aspose.gridweb/gridvalidation) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取枚举器的大小 |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | 获取应用于给定单元格的验证。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 删除指定索引处的验证。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public GridValidation add()
```


向集合中添加一个 [GridValidation](../../com.aspose.gridweb/gridvalidation)。

**Remarks**

注意：此成员已过时。请改用 GridValidationCollection.Add(row,col) 方法。此属性将在自 2015 年 1 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(GridCellArea ca) {#add-com.aspose.gridweb.GridCellArea-}
```
public GridValidation add(GridCellArea ca)
```


向集合添加数据验证。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 该区域包含此验证。 |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the validation.
### add(GridValidation validation) {#add-com.aspose.gridweb.GridValidation-}
```
public int add(GridValidation validation)
```


向集合中添加一个 [GridValidation](../../com.aspose.gridweb/gridvalidation)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| validation | [GridValidation](../../com.aspose.gridweb/gridvalidation) | 一个验证对象。 |

**Returns:**
int - [GridValidation](../../com.aspose.gridweb/gridvalidation) 对象索引。
### add(int row, int column) {#add-int-int-}
```
public GridValidation add(int row, int column)
```


向集合中添加一个 [GridValidation](../../com.aspose.gridweb/gridvalidation)。验证将应用于指定的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(String cellname) {#add-java.lang.String-}
```
public GridValidation add(String cellname)
```


向集合中添加一个 [GridValidation](../../com.aspose.gridweb/gridvalidation)。验证将应用于指定的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellname | java.lang.String | 单元格的名称。 |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### clear() {#clear--}
```
public void clear()
```


清除所有验证。

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
public GridValidation get(int index)
```


获取指定索引处的 [GridValidation](../../com.aspose.gridweb/gridvalidation) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - The element at the specified index.
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
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public GridValidation getValidationInCell(int row, int column)
```


获取应用于给定单元格的验证。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - Returns a [GridValidation](../../com.aspose.gridweb/gridvalidation) object or null if there is no validation for given cell
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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


删除指定索引处的验证。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

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

