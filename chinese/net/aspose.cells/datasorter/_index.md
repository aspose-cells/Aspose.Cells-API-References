---
title: DataSorter
second_title: Aspose.Cells for .NET API 参考
description: DataSorter 的摘要描述
type: docs
weight: 1300
url: /zh/net/aspose.cells/datasorter/
---
## DataSorter class

DataSorter 的摘要描述。

```csharp
public class DataSorter
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive) { get; set; } | 获取和设置比较字符串时是否区分大小写。 |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders) { get; set; } | 表示范围是否有headers。 |
| [Key1](../../aspose.cells/datasorter/key1) { get; set; } | 表示第一个排好序的列索引（绝对位置，A 列为 0，B 为 1，...）。 |
| [Key2](../../aspose.cells/datasorter/key2) { get; set; } | 表示第二个排好序的列索引（绝对位置，A列为0，B为1，...）。 |
| [Key3](../../aspose.cells/datasorter/key3) { get; set; } | 表示第三个排好序的列索引（绝对位置，A列为0，B为1，...）。 |
| [Keys](../../aspose.cells/datasorter/keys) { get; } | 获取数据排序器的键列表。 |
| [Order1](../../aspose.cells/datasorter/order1) { get; set; } | 表示第一个键的排序顺序。 |
| [Order2](../../aspose.cells/datasorter/order2) { get; set; } | 表示第二个key的排序顺序。 |
| [Order3](../../aspose.cells/datasorter/order3) { get; set; } | 表示第三个key的排序顺序。 |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber) { get; set; } | 指示是否对任何看起来像数字的东西进行排序。 |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright) { get; set; } | True 表示排序方向是从左到右。 False 表示排序方向是从上到下。 默认值为false。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_1)(int, SortOrder) | 添加排好序的列索引和排序顺序。 |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_2)(int, SortOrder, string) | 使用自定义排序列表添加排序的列索引和排序顺序。 |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_3)(int, SortOrder, string[]) | 使用自定义排序列表添加排序的列索引和排序顺序。 |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey)(int, SortOnType, SortOrder, object) | 使用自定义排序列表添加排序的列索引和排序顺序。 |
| [Clear](../../aspose.cells/datasorter/clear)() | 清除所有设置。 |
| [Sort](../../aspose.cells/datasorter/sort#sort)() | 对范围内的数据进行排序。 |
| [Sort](../../aspose.cells/datasorter/sort#sort_1)(Cells, CellArea) | 对该区域的数据进行排序 |
| [Sort](../../aspose.cells/datasorter/sort#sort_2)(Cells, int, int, int, int) | 对该区域的数据进行排序。 |

### 例子

```csharp

[C#]

//实例化一个新的 Workbook 对象。
Workbook workbook = new Workbook("Book1.xls");
//获取工作簿数据排序器对象。
DataSorter sorter = workbook.DataSorter;
//设置数据排序器对象的第一顺序。
sorter.Order1 = Aspose.Cells.SortOrder.Descending;
//定义第一个键。
sorter.Key1 = 0;
//设置数据排序器对象的第二个顺序。
sorter.Order2 = Aspose.Cells.SortOrder.Ascending;
//定义第二个键。
sorter.Key2 = 1;
//创建一个单元格区域（范围）。
CellArea ca = new CellArea();
//指定起始行索引。
ca.StartRow = 0;
//指定起始列索引。
ca.StartColumn = 0;
//指定最后一行索引。
ca.EndRow = 13;
//指定最后一列索引。
ca.EndColumn = 1;
//对指定数据范围内的数据进行排序（A1:B14）
sorter.Sort(workbook.Worksheets[0].Cells, ca);
//保存excel文件。
workbook.Save("outBook.xls");

[Visual Basic]

'实例化一个新的 Workbook 对象。
Dim workbook As Workbook = New Workbook("Book1.xls")
'获取工作簿数据排序器对象。
Dim sorter As DataSorter = workbook.DataSorter
'设置数据排序器对象的第一顺序
sorter.Order1 = Aspose.Cells.SortOrder.Descending
'定义第一个键。
sorter.Key1 = 0
'设置数据排序器对象的第二个顺序。
sorter.Order2 = Aspose.Cells.SortOrder.Ascending
'定义第二个键。
sorter.Key2 = 1
'创建一个单元格区域（范围）。
Dim ca As CellArea = New CellArea
'指定起始行索引。
ca.StartRow = 0
'指定起始列索引。
ca.StartColumn = 0
'指定最后一行索引。
ca.EndRow = 13
'指定最后一列索引。
ca.EndColumn = 1
'对指定数据范围内的数据进行排序（A1:B14）
sorter.Sort(workbook.Worksheets(0).Cells, ca)
'保存excel文件。
workbook.Save("outBook.xls")

```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
