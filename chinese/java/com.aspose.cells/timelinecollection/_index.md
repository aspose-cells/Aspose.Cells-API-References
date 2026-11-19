---
title: "TimelineCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "指定工作表上所有对象的集合。"
type: docs
url: /zh/java/com.aspose.cells/timelinecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TimelineCollection extends CollectionBase
```

指定工作表上所有 [Timeline](../../com.aspose.cells/timeline) 对象的集合。自 Excel 2013 起受支持。

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
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | 使用透视表作为数据源添加新的 Timeline |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | 使用透视表作为数据源添加新的 Timeline |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | 使用透视表作为数据源添加新的 Timeline |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | 使用透视表作为数据源添加新的 Timeline |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | 使用透视表作为数据源添加新的 Timeline |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | 使用透视表作为数据源添加新的 Timeline |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 按索引获取 Timeline。 |
| [get(String name)](#get-java.lang.String-) | 按 Timeline 名称获取 Timeline。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的项。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


使用透视表作为数据源添加新的 Timeline

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 20, 5, pivot.getBaseFields().get(1));
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| 行 | int | Timeline 区域左上角单元格的行索引。 |
| 列 | int | Timeline 区域左上角单元格的列索引。 |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | PivotTable.BaseFields 中的 PivotField |

**Returns:**
int - 新添加的 Timeline 索引
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


使用透视表作为数据源添加新的 Timeline

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 15, 5, 1);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| 行 | int | Timeline 区域左上角单元格的行索引。 |
| 列 | int | Timeline 区域左上角单元格的列索引。 |
| baseFieldIndex | int | PivotTable.BaseFields 中 PivotField 的索引 |

**Returns:**
int - 新添加的 Timeline 索引
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


使用透视表作为数据源添加新的 Timeline

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 10, 5, "date");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| 行 | int | Timeline 区域左上角单元格的行索引。 |
| 列 | int | Timeline 区域左上角单元格的列索引。 |
| baseFieldName | java.lang.String | PivotTable.BaseFields 中 PivotField 的名称 |

**Returns:**
int - 新添加的 Timeline 索引
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


使用透视表作为数据源添加新的 Timeline

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i10", pivot.getBaseFields().get(1));
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| destCellName | java.lang.String | Timeline 区域左上角单元格的名称。 |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | PivotTable.BaseFields 中的 PivotField |

**Returns:**
int - 新添加的 Timeline 索引
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


使用透视表作为数据源添加新的 Timeline

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i5", 1);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| destCellName | java.lang.String | Timeline 区域左上角单元格的名称。 |
| baseFieldIndex | int | PivotTable.BaseFields 中 PivotField 的索引 |

**Returns:**
int - 新添加的 Timeline 索引
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


使用透视表作为数据源添加新的 Timeline

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i15", "date");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| destCellName | java.lang.String | Timeline 区域左上角单元格的名称。 |
| baseFieldName | java.lang.String | PivotTable.BaseFields 中 PivotField 的名称 |

**Returns:**
int - 新添加的 Timeline 索引
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
public Timeline get(int index)
```


按索引获取 Timeline。

**Example**

```
         //Get the Timeline by index.
         Timeline objByIndex = sheet.getTimelines().get(0);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
[Timeline](../../com.aspose.cells/timeline)
### get(String name) {#get-java.lang.String-}
```
public Timeline get(String name)
```


按 Timeline 名称获取 Timeline。

**Example**

```
         //Get the Timeline by Timeline's name.
         Timeline objByName = sheet.getTimelines().get("date");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[Timeline](../../com.aspose.cells/timeline)
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

