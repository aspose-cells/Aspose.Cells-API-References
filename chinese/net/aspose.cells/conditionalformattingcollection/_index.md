---
title: ConditionalFormattingCollection
second_title: Aspose.Cells for .NET API 参考
description: 封装FormatCondition./formatcondition对象的集合
type: docs
weight: 1100
url: /zh/net/aspose.cells/conditionalformattingcollection/
---
## ConditionalFormattingCollection class

封装[`FormatCondition`](../formatcondition)对象的集合。

```csharp
public class ConditionalFormattingCollection : CollectionBase<FormatConditionCollection>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingcollection/item) { get; } | 获取指定索引处的 FormatConditions 元素。 |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingcollection/add)() | 将 FormatConditions 添加到集合中。 |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(FormatConditionCollection) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(FormatConditionCollection) |  |
| [Copy](../../aspose.cells/conditionalformattingcollection/copy)(ConditionalFormattingCollection) | 复制条件格式。 |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(FormatConditionCollection[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(FormatConditionCollection[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, FormatConditionCollection[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection, int, int) |  |
| [RemoveArea](../../aspose.cells/conditionalformattingcollection/removearea)(int, int, int, int) | 删除范围内的所有条件格式。 |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### 例子

```csharp

[C#]

 //实例化一个工作簿对象
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//获取条件格式
ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;

 //添加一个空的条件格式
int index = cformattings.Add();

 //获取新添加的条件格式
FormatConditionCollection fcs = cformattings[index];

 //设置条件格式范围.
CellArea ca = new CellArea();

ca.StartRow = 0;

ca.EndRow = 0;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

ca = new CellArea();

ca.StartRow = 1;

ca.EndRow = 1;

ca.StartColumn = 1;

ca.EndColumn = 1;

fcs.AddArea(ca);

 //添加条件.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");

 //添加条件.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

 //设置背景颜色.
FormatCondition fc = fcs[conditionIndex];

fc.Style.BackgroundColor = Color.Red;

 //保存Excel文件
workbook.Save("output.xls");

[VB.NET]

'Instantiating a Workbook object
DDim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Get Conditional Formatting
Dim cformattings As ConditionalFormattingCollection = sheet.ConditionalFormattings

'Adds an empty conditional formatting
Dim index As Integer = cformattings.Add()

'Get newly added Conditional formatting
Dim fcs As FormatConditionCollection = cformattings(index)

'Sets the conditional format range.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 0

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

ca = New CellArea()

ca.StartRow = 1

ca.EndRow = 1

ca.StartColumn = 1

ca.EndColumn = 1

fcs.AddArea(ca)

'Add condition.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")

'Add condition.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")

'Sets the background color.
Dim fc As FormatCondition = fcs(conditionIndex)

fc.Style.BackgroundColor = Color.Red

'Saving the Excel file
workbook.Save("output.xls")
```

### 也可以看看

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [FormatConditionCollection](../formatconditioncollection)
* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
