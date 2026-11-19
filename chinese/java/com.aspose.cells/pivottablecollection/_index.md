---
title: "PivotTableCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示指定工作表上所有 PivotTable 对象的集合。"
type: docs
url: /zh/java/com.aspose.cells/pivottablecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableCollection extends CollectionBase
```

表示指定工作表上所有 PivotTable 对象的集合。

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
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(PivotTable pivotTable, int row, int column, String tableName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | 基于另一个数据透视表添加一个新数据透视表。 |
| [add(PivotTable pivotTable, String destCellName, String tableName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | 基于另一个数据透视表添加一个新数据透视表。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [add(String sourceData, int row, int column)](#add-java.lang.String-int-int-) | 在指定的工作表行列位置添加一个新的现代数据透视表（自 Excel 2007 起），使用默认选项。 |
| [add(String sourceData, int row, int column, PivotTableCreateOptions options)](#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-) | 在指定的工作表行列位置添加一个新数据透视表。 |
| [add(String sourceData, int row, int column, String tableName)](#add-java.lang.String-int-int-java.lang.String-) | 使用传统的 Excel 97-2003 布局和样式添加一个新数据透视表。 |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource)](#add-java.lang.String-int-int-java.lang.String-boolean-) | 使用传统的 Excel 97-2003 布局和样式添加一个新数据透视表。 |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-int-int-java.lang.String-boolean-boolean-) | 使用传统的 Excel 97-2003 布局和样式添加一个新数据透视表。 |
| [add(String sourceData, String cellName)](#add-java.lang.String-java.lang.String-) | 在指定的工作表行列位置添加一个新的现代数据透视表（自 Excel 2007 起），使用默认选项。 |
| [add(String sourceData, String cellName, PivotTableCreateOptions options)](#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-) | 在指定的工作表行列位置添加一个新的现代数据透视表（自 Excel 2007 起），使用默认选项。 |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | 使用传统的 Excel 97-2003 布局和样式添加一个新数据透视表。 |
| [add(String sourceData, String destCellName, String tableName, boolean useSameSource)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-) | 使用传统的 Excel 97-2003 布局和样式添加一个新数据透视表。 |
| [add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-) | 添加一个新数据透视表。 |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-) | 向集合中添加一个新的数据透视表对象，使用多个合并范围作为数据源。 |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-) | 向集合中添加一个新的数据透视表对象，使用多个合并范围作为数据源。 |
| [clear()](#clear--) | 清除所有数据透视表。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [dispose()](#dispose--) | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 按索引获取数据透视表报告。 |
| [get(int row, int column)](#get-int-int-) | 获取位于单元格中的 [PivotTable](../../com.aspose.cells/pivottable)。 |
| [get(String name)](#get-java.lang.String-) | 按数据透视表名称获取报告。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotTable pivotTable)](#remove-com.aspose.cells.PivotTable-) | 删除指定的数据透视表并删除其数据。 |
| [remove(PivotTable pivotTable, boolean keepData)](#remove-com.aspose.cells.PivotTable-boolean-) | 删除指定的数据透视表。 |
| [removeAt(int index)](#removeAt-int-) | 删除指定索引处的数据透视表并删除其数据。 |
| [removeAt(int index, boolean keepData)](#removeAt-int-boolean-) | 删除指定索引处的 PivotTable |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivotTable, int row, int column, String tableName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivotTable, int row, int column, String tableName)
```


基于另一个数据透视表添加一个新数据透视表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | 源 PivotTable。 |
| 行 | int | PivotTable 报表目标范围左上角单元格的行索引。 |
| 列 | int | PivotTable 报表目标范围左上角单元格的列索引。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |

**Returns:**
int - 新添加的 PivotTable 索引。
### add(PivotTable pivotTable, String destCellName, String tableName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivotTable, String destCellName, String tableName)
```


基于另一个数据透视表添加一个新数据透视表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | 源 PivotTable。 |
| destCellName | java.lang.String | PivotTable 报表目标范围左上角的单元格。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |

**Returns:**
int - 新添加的 PivotTable 索引。
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
### add(String sourceData, int row, int column) {#add-java.lang.String-int-int-}
```
public PivotTable add(String sourceData, int row, int column)
```


在指定的工作表行列位置添加一个新的现代数据透视表（自 Excel 2007 起），使用默认选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String | 新 PivotTable 的数据单元格范围。示例：Sheet1!A1:C8 |
| 行 | int | PivotTable 目标左上角的零基行索引。 |
| 列 | int | PivotTable 目标左上角的零基列索引。 |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, PivotTableCreateOptions options) {#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, int row, int column, PivotTableCreateOptions options)
```


在指定的工作表行列位置添加一个新数据透视表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String | 新 PivotTable 的数据单元格范围。示例：Sheet1!A1:C8 |
| 行 | int | PivotTable 目标左上角的零基行索引。 |
| 列 | int | PivotTable 目标左上角的零基列索引。 |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | PivotTable 创建选项。 |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, String tableName) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String sourceData, int row, int column, String tableName)
```


使用传统的 Excel 97-2003 布局和样式添加一个新数据透视表。

**Remarks**

注意：此方法已过时。它等同于使用 `NewPivotTableOptions.IsXlsClassic = true` 调用 PivotTableCollection.Add(string, int, int, PivotTableCreateOptions)。请改用 PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) 重载。此方法将在 2026 年 9 月后 12 个月被移除。对造成的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String | 新 PivotTable 的数据单元格范围。示例：Sheet1!A1:C8 |
| 行 | int | PivotTable 报表目标范围左上角单元格的行索引。 |
| 列 | int | PivotTable 报表目标范围左上角单元格的列索引。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |

**Returns:**
int - 此 pivot table 列表中的索引。
### add(String sourceData, int row, int column, String tableName, boolean useSameSource) {#add-java.lang.String-int-int-java.lang.String-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource)
```


使用传统的 Excel 97-2003 布局和样式添加一个新数据透视表。

**Remarks**

注意：此方法已过时。它等同于使用 `NewPivotTableOptions.IsXlsClassic = true` 调用 PivotTableCollection.Add(string, int, int, PivotTableCreateOptions)。请改用 PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) 重载。此方法将在 2026 年 9 月后 12 个月被移除。对造成的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String | 新 PivotTable 的数据单元格范围。示例：Sheet1!A1:C8 |
| 行 | int | PivotTable 报表目标范围左上角单元格的行索引。 |
| 列 | int | PivotTable 报表目标范围左上角单元格的列索引。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |
| useSameSource | boolean | 指示在另一个已有的 pivot table 已使用该数据源时是否使用相同的数据源。如果属性为 true，则可节省内存。 |

**Returns:**
int - 新添加的缓存索引。
### add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-int-int-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)
```


使用传统的 Excel 97-2003 布局和样式添加一个新数据透视表。

**Remarks**

注意：此方法已过时。它等同于使用 `NewPivotTableOptions.IsXlsClassic = true` 调用 PivotTableCollection.Add(string, int, int, PivotTableCreateOptions)。请改用 PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) 重载。此方法将在 2026 年 10 月后 12 个月被移除。对造成的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String | 新 PivotTable 的数据单元格范围。示例：Sheet1!A1:C8 |
| 行 | int | PivotTable 报表目标范围左上角单元格的行索引。 |
| 列 | int | PivotTable 报表目标范围左上角单元格的列索引。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |
| useSameSource | boolean | 指示在另一个已有的 pivot table 已使用该数据源时是否使用相同的数据源。如果属性为 true，则可节省内存。 |
| isXlsClassic | boolean | 指示是否添加 Excel 97-2003 经典 PivotTable。 |

**Returns:**
int - 新添加的缓存索引。
### add(String sourceData, String cellName) {#add-java.lang.String-java.lang.String-}
```
public PivotTable add(String sourceData, String cellName)
```


在指定的工作表行列位置添加一个新的现代数据透视表（自 Excel 2007 起），使用默认选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String | 新 PivotTable 的数据单元格范围。示例：Sheet1!A1:C8 |
| cellName | java.lang.String | PivotTable 目标左上角单元格的名称。 |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String cellName, PivotTableCreateOptions options) {#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, String cellName, PivotTableCreateOptions options)
```


在指定的工作表行列位置添加一个新的现代数据透视表（自 Excel 2007 起），使用默认选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String | 新 PivotTable 的数据单元格范围。示例：Sheet1!A1:C8 |
| cellName | java.lang.String | PivotTable 目标左上角单元格的名称。 |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | 创建 pivot table 的选项。 |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


使用传统的 Excel 97-2003 布局和样式添加一个新数据透视表。

**Remarks**

注意：此方法已过时。它等同于使用 `NewPivotTableOptions.IsXlsClassic = true` 调用 PivotTableCollection.Add(string, int, int, PivotTableCreateOptions)。请改用 PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) 重载。此方法将在 2026 年 9 月后 12 个月被移除。对造成的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String | 新 PivotTable 缓存的数据。 |
| destCellName | java.lang.String | PivotTable 报表目标范围左上角的单元格。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |

**Returns:**
int - 此 pivot table 列表中的索引。
### add(String sourceData, String destCellName, String tableName, boolean useSameSource) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public int add(String sourceData, String destCellName, String tableName, boolean useSameSource)
```


使用传统的 Excel 97-2003 布局和样式添加一个新数据透视表。

**Remarks**

注意：此方法已过时。它等同于使用 `NewPivotTableOptions.IsXlsClassic = true` 调用 PivotTableCollection.Add(string, int, int, PivotTableCreateOptions)。请改用 PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) 重载。此方法将在 2026 年 9 月后 12 个月被移除。对造成的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String | 新 PivotTable 缓存的数据。 |
| destCellName | java.lang.String | PivotTable 报表目标范围左上角的单元格。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |
| useSameSource | boolean | 指示在另一个已有的 pivot table 已使用该数据源时是否使用相同的数据源。如果属性为 true，则可节省内存。 |

**Returns:**
int - 新添加的缓存索引。
### add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)
```


添加一个新数据透视表。

**Remarks**

注意：此方法已过时。它等同于使用 `NewPivotTableOptions.IsXlsClassic = true` 调用 PivotTableCollection.Add(string, int, int, PivotTableCreateOptions)。请改用 PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) 重载。此方法将在 2026 年 10 月后 12 个月被移除。对造成的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String | 新 PivotTable 的数据单元格范围。示例：Sheet1!A1:C8 |
| cell | java.lang.String | PivotTable 报表目标范围左上角的单元格。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |
| useSameSource | boolean | 指示在另一个已存在的透视表已使用此数据源时，是否使用相同的数据源。如果属性为 true，则在相同的数据源被汇集到一个透视缓存中时可节省内存。 |
| isXlsClassic | boolean | 指示是否添加 Excel 97-2003 经典 PivotTable。 |

**Returns:**
int - 新添加的缓存索引。
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)
```


向集合中添加一个新的数据透视表对象，使用多个合并范围作为数据源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String[] | 多个合并范围，例如 \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | 是否自动创建单页字段。如果为 true，以下参数 pageFields 将被忽略 |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | 透视页字段项。 |
| 行 | int | PivotTable 报表目标范围左上角单元格的行索引。 |
| 列 | int | PivotTable 报表目标范围左上角单元格的列索引。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |

**Returns:**
int - 新添加的 PivotTable 索引。
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)
```


向集合中添加一个新的数据透视表对象，使用多个合并范围作为数据源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String[] | 多个合并范围，例如 \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | 是否自动创建单页字段。如果为 true，以下参数 pageFields 将被忽略。 |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | 透视页字段项。 |
| destCellName | java.lang.String | destCellName 新透视表报告的名称。 |
| tableName | java.lang.String | 新透视表报告的名称。 |

**Returns:**
int - 新添加的 PivotTable 索引。
### clear() {#clear--}
```
public void clear()
```


清除所有数据透视表。

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
### dispose() {#dispose--}
```
public void dispose()
```


执行应用程序定义的任务，以释放、释放或重置非托管资源。

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
public PivotTable get(int index)
```


按索引获取数据透视表报告。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(int row, int column) {#get-int-int-}
```
public PivotTable get(int row, int column)
```


获取位于单元格中的 [PivotTable](../../com.aspose.cells/pivottable)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int |  |
| 列 | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(String name) {#get-java.lang.String-}
```
public PivotTable get(String name)
```


按数据透视表名称获取报告。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
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




### remove(PivotTable pivotTable) {#remove-com.aspose.cells.PivotTable-}
```
public void remove(PivotTable pivotTable)
```


删除指定的数据透视表并删除其数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |

### remove(PivotTable pivotTable, boolean keepData) {#remove-com.aspose.cells.PivotTable-boolean-}
```
public void remove(PivotTable pivotTable, boolean keepData)
```


删除指定的数据透视表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |
| keepData | boolean | 是否保留透视表数据 |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


删除指定索引处的数据透视表并删除其数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 在透视表集合中的位置索引 |

### removeAt(int index, boolean keepData) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean keepData)
```


删除指定索引处的 PivotTable

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 在透视表集合中的位置索引 |
| keepData | boolean | 是否保留透视表数据 |

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

