---
title: "ValidationCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示数据验证集合。"
type: docs
url: /zh/java/com.aspose.cells/validationcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ValidationCollection extends CollectionBase
```

表示数据验证集合。

**Example**

```
         Workbook workbook = new Workbook();
         	ValidationCollection validations = workbook.getWorksheets().get(0).getValidations();
         CellArea area = CellArea.createCellArea(0, 0, 1, 1);
         Validation validation = validations.get(validations.add(area));
         validation.setType(com.aspose.cells.ValidationType.LIST);
         validation.setFormula1("a,b,c,d");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add()](#add--) | 向集合添加数据验证。 |
| [add(CellArea ca)](#add-com.aspose.cells.CellArea-) | 向集合添加数据验证。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取位于指定索引的 [Validation](../../com.aspose.cells/validation) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | 获取应用于给定单元格的验证。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | 删除单元格上的所有验证设置。 |
| [removeArea(CellArea ca)](#removeArea-com.aspose.cells.CellArea-) | 删除范围上的所有验证设置.. |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的项。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


向集合添加数据验证。

**Remarks**

注意：此方法现已过时。请改用 ValidationCollection.Add(CellArea) 方法。该方法将在自 2015 年 1 月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
int - [Validation](../../com.aspose.cells/validation) 对象索引。
### add(CellArea ca) {#add-com.aspose.cells.CellArea-}
```
public int add(CellArea ca)
```


向集合添加数据验证。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 该区域包含此验证。 |

**Returns:**
int - [Validation](../../com.aspose.cells/validation) 对象索引。
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
public Validation get(int index)
```


获取位于指定索引的 [Validation](../../com.aspose.cells/validation) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[Validation](../../com.aspose.cells/validation) - The element at the specified index.
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
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public Validation getValidationInCell(int row, int column)
```


获取应用于给定单元格的验证。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
[Validation](../../com.aspose.cells/validation) - Returns a [Validation](../../com.aspose.cells/validation) object or null if there is no validation for given cell
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




### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```


删除单元格上的所有验证设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 单元格的行索引。 |
| 列 | int | 单元格的列索引。 |

### removeArea(CellArea ca) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea ca)
```


删除范围上的所有验证设置..

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 包含验证设置的范围。 |

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

