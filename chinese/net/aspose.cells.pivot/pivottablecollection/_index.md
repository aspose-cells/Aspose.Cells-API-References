---
title: PivotTableCollection
second_title: Aspose.Cells for .NET API 参考
description: 表示指定工作表上所有数据透视表对象的集合
type: docs
weight: 4710
url: /zh/net/aspose.cells.pivot/pivottablecollection/
---
## PivotTableCollection class

表示指定工作表上所有数据透视表对象的集合。

```csharp
public class PivotTableCollection : CollectionBase<PivotTable>, IDisposable
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.pivot/pivottablecollection/item) { get; } | 按索引获取数据透视表。 (3 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_1)(PivotTable, string, string) | 将新的数据透视表对象从另一个数据透视表添加到集合中。 |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_4)(string, string, string) | 将新的数据透视表缓存添加到 PivotCaches 集合。 |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add)(PivotTable, int, int, string) | 将新的数据透视表对象从另一个数据透视表添加到集合中。 |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_2)(string, int, int, string) | 将新的数据透视表缓存添加到 PivotCaches 集合。 |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_5)(string, string, string, bool) | 将新的数据透视表缓存添加到 PivotCaches 集合。 |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_3)(string, int, int, string, bool) | 将新的数据透视表缓存添加到 PivotCaches 集合。 |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_7)(string[], bool, PivotPageFields, string, string) | 将一个新的数据透视表对象添加到具有多个合并范围作为数据源的集合中。 |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_6)(string[], bool, PivotPageFields, int, int, string) | 将一个新的数据透视表对象添加到具有多个合并范围作为数据源的集合中。 |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(PivotTable) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(PivotTable, IComparer&lt;PivotTable&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, PivotTable, IComparer&lt;PivotTable&gt;) |  |
| [Clear](../../aspose.cells.pivot/pivottablecollection/clear#clear)() | 清除所有数据透视表。 (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(PivotTable) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(PivotTable[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(PivotTable[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, PivotTable[], int, int) |  |
| [Dispose](../../aspose.cells.pivot/pivottablecollection/dispose)() | 执行与释放、释放或 重置非托管资源相关的应用程序定义任务。 |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;PivotTable&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;PivotTable&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;PivotTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;PivotTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;PivotTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;PivotTable&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;PivotTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;PivotTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;PivotTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;PivotTable&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(PivotTable) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(PivotTable, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(PivotTable, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(PivotTable) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(PivotTable, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(PivotTable, int, int) |  |
| [Remove](../../aspose.cells.pivot/pivottablecollection/remove#remove)(PivotTable) | 删除指定数据透视表并删除数据透视表数据 |
| [Remove](../../aspose.cells.pivot/pivottablecollection/remove#remove_1)(PivotTable, bool) | 删除指定的数据透视表 |
| [RemoveAt](../../aspose.cells.pivot/pivottablecollection/removeat#removeat)(int) | 删除指定索引处的数据透视表并删除数据透视表数据 (2 methods) |
| [RemoveAt](../../aspose.cells.pivot/pivottablecollection/removeat#removeat_2)(int, bool) | 删除指定索引处的数据透视表 |

### 例子

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

 //改变PivotField的属性
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

 //添加PivotFilter
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

 //添加PivotFormatCondition
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

 //做你的事

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Add PivotFilter
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

'Add PivotFormatCondition
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### 也可以看看

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [PivotTable](../pivottable)
* 命名空间 [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
