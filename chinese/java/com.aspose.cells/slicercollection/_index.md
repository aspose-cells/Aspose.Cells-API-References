---
title: "SlicerCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "指定工作表上所有切片器对象的集合。"
type: docs
url: /zh/java/com.aspose.cells/slicercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SlicerCollection extends CollectionBase
```

指定工作表上所有切片器对象的集合。

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
 
         //do your business
 
         book.save("out.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(ListObject table, ListColumn listColumn, int row, int column)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-) | 使用 ListObjet 作为数据源添加新的切片器。 |
| [add(ListObject table, ListColumn listColumn, String destCellName)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-) | 使用 ListObjet 作为数据源添加新的切片器。 |
| [add(ListObject table, int index, String destCellName)](#add-com.aspose.cells.ListObject-int-java.lang.String-) | 使用 ListObjet 作为数据源添加新的切片器。 |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | 使用 PivotTable 作为数据源添加新的切片器。 |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | 使用 PivotTable 作为数据源添加新的切片器。 |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | 使用 PivotTable 作为数据源添加新的切片器。 |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | 使用 PivotTable 作为数据源添加新的切片器。 |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | 使用 PivotTable 作为数据源添加新的切片器。 |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | 使用 PivotTable 作为数据源添加新的切片器。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [clear()](#clear--) | 清除所有切片器。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 通过索引获取切片器。 |
| [get(String name)](#get-java.lang.String-) | 通过切片器名称获取切片器。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Slicer slicer)](#remove-com.aspose.cells.Slicer-) | 移除指定的切片器 |
| [removeAt(int index)](#removeAt-int-) | 删除指定索引处的切片器 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ListObject table, ListColumn listColumn, int row, int column) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-}
```
public int add(ListObject table, ListColumn listColumn, int row, int column)
```


使用 ListObjet 作为数据源添加新的切片器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject 对象 |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | ListObject.ListColumns 中的 ListColumn |
| 行 | int | 切片器范围左上角单元格的行索引。 |
| 列 | int | 切片器范围左上角单元格的列索引。 |

**Returns:**
int - 新添加的切片器索引
### add(ListObject table, ListColumn listColumn, String destCellName) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-}
```
public int add(ListObject table, ListColumn listColumn, String destCellName)
```


使用 ListObjet 作为数据源添加新的切片器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject 对象 |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | ListObject.ListColumns 中的 ListColumn |
| destCellName | java.lang.String | 切片器范围左上角的单元格。 |

**Returns:**
int - 新添加的切片器索引
### add(ListObject table, int index, String destCellName) {#add-com.aspose.cells.ListObject-int-java.lang.String-}
```
public int add(ListObject table, int index, String destCellName)
```


使用 ListObjet 作为数据源添加新的切片器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject 对象 |
| 索引 | int | ListObject.ListColumns 中 ListColumn 的索引 |
| destCellName | java.lang.String | 切片器范围左上角的单元格。 |

**Returns:**
int - 新添加的切片器索引
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


使用 PivotTable 作为数据源添加新的切片器。

**Example**

```
         slicers.add(pivot, 3, 12, pivot.getBaseFields().get(0));
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| 行 | int | 切片器范围左上角单元格的行索引。 |
| 列 | int | 切片器范围左上角单元格的列索引。 |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | PivotTable.BaseFields 中的 PivotField |

**Returns:**
int - 新添加的切片器索引
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


使用 PivotTable 作为数据源添加新的切片器。

**Example**

```
         slicers.add(pivot, 20, 8, 0);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| 行 | int | 切片器范围左上角单元格的行索引。 |
| 列 | int | 切片器范围左上角单元格的列索引。 |
| baseFieldIndex | int | PivotTable.BaseFields 中 PivotField 的索引 |

**Returns:**
int - 新添加的切片器索引
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


使用 PivotTable 作为数据源添加新的切片器。

**Example**

```
         slicers.add(pivot, 20, 12, "fruit");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| 行 | int | 切片器范围左上角单元格的行索引。 |
| 列 | int | 切片器范围左上角单元格的列索引。 |
| baseFieldName | java.lang.String | PivotTable.BaseFields 中 PivotField 的名称 |

**Returns:**
int - 新添加的切片器索引
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


使用 PivotTable 作为数据源添加新的切片器。

**Example**

```
         slicers.add(pivot, "I3", pivot.getBaseFields().get(0));
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| destCellName | java.lang.String | 切片器范围左上角的单元格。 |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | PivotTable.BaseFields 中的 PivotField |

**Returns:**
int - 新添加的切片器索引
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


使用 PivotTable 作为数据源添加新的切片器。

**Example**

```
         slicers.add(pivot, "E20", 0);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| destCellName | java.lang.String | 切片器范围左上角的单元格。 |
| baseFieldIndex | int | PivotTable.BaseFields 中 PivotField 的索引 |

**Returns:**
int - 新添加的切片器索引
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


使用 PivotTable 作为数据源添加新的切片器。

**Example**

```
         slicers.add(pivot, "E3", "fruit");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| destCellName | java.lang.String | 切片器范围左上角的单元格。 |
| baseFieldName | java.lang.String | PivotTable.BaseFields 中 PivotField 的名称 |

**Returns:**
int - 新添加的切片器索引
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


清除所有切片器。

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
public Slicer get(int index)
```


通过索引获取切片器。

**Example**

```
         Slicer slicerByIndex = slicers.get(0);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
### get(String name) {#get-java.lang.String-}
```
public Slicer get(String name)
```


通过切片器名称获取切片器。

**Example**

```
         Slicer slicerByName = slicers.get("fruit");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
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




### remove(Slicer slicer) {#remove-com.aspose.cells.Slicer-}
```
public void remove(Slicer slicer)
```


移除指定的切片器

**Example**

```
         Slicer delSlicer = slicers.get(0);
         slicers.remove(delSlicer);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| slicer | [Slicer](../../com.aspose.cells/slicer) | Slicer 对象 |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


删除指定索引处的切片器

**Example**

```
         slicers.removeAt(1);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | Slicer 集合中的位置索引 |

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

