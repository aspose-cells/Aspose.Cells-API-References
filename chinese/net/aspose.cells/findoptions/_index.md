---
title: FindOptions
second_title: Aspose.Cells for .NET API 参考
description: 表示查找选项
type: docs
weight: 3470
url: /zh/net/aspose.cells/findoptions/
---
## FindOptions class

表示查找选项。

```csharp
public class FindOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [FindOptions](findoptions)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [CaseSensitive](../../aspose.cells/findoptions/casesensitive) { get; set; } | 指示搜索的字符串是否区分大小写。 |
| [ConvertNumericData](../../aspose.cells/findoptions/convertnumericdata) { get; set; } | 获取或设置一个值，该值指示是否将搜索到的字符串值转换为数值数据。 |
| [IsRangeSet](../../aspose.cells/findoptions/israngeset) { get; } | 表示是否设置了搜索范围。 |
| [LookAtType](../../aspose.cells/findoptions/lookattype) { get; set; } | 看类型。 |
| [LookInType](../../aspose.cells/findoptions/lookintype) { get; set; } | 查找类型。 |
| [RegexKey](../../aspose.cells/findoptions/regexkey) { get; set; } | 表示搜索到的键是否是正则表达式。如果为真，则搜索到的键将被视为正则表达式。 |
| [SeachOrderByRows](../../aspose.cells/findoptions/seachorderbyrows) { get; set; } | 表示是按行还是按列搜索。 |
| [SearchBackward](../../aspose.cells/findoptions/searchbackward) { get; set; } | 是否向后搜索单元格。 |
| [Style](../../aspose.cells/findoptions/style) { get; set; } | 要搜索的格式。 |
| [ValueTypeSensitive](../../aspose.cells/findoptions/valuetypesensitive) { get; set; } | 指示搜索的单元格值类型是否应与搜索的键相同。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [GetRange](../../aspose.cells/findoptions/getrange)() | 获取和设置搜索范围。 |
| [SetRange](../../aspose.cells/findoptions/setrange)(CellArea) | 设置搜索范围。 |

### 例子

```csharp

[C#]

 //实例化工作簿对象
Workbook workbook = new Workbook("book1.xls");

 //获取Cells集合
Cells cells = workbook.Worksheets[0].Cells;

 //实例化 FindOptions Object
FindOptions findOptions = new FindOptions();

 //创建一个Cells Area
CellArea ca = new CellArea();
ca.StartRow = 8;
ca.StartColumn = 2;
ca.EndRow = 17;
ca.EndColumn = 13;

 //为查找选项设置单元格区域
findOptions.SetRange(ca);

 //设置搜索属性
findOptions.SearchBackward = false;

findOptions.SeachOrderByRows = true;

findOptions.LookInType = LookInType.Values;

 //找到值为0的单元格
Cell cell = cells.Find(0, null, findOptions);

[VB.NET]

'Instantiate the workbook object
Dim workbook As New Workbook("book1.xls")

'Get Cells collection 
Dim cells As Cells = workbook.Worksheets(0).Cells

'Instantiate FindOptions Object
Dim findOptions As New FindOptions()

'Create a Cells Area
Dim ca As New CellArea()
ca.StartRow = 8
ca.StartColumn = 2
ca.EndRow = 17
ca.EndColumn = 13

'Set cells area for find options
findOptions.SetRange(ca)

'Set searching properties
findOptions.SearchBackward = True

findOptions.SeachOrderByRows = True

findOptions.LookInType = LookInType.Values

'Find the cell with 0 value
Dim cell As Cell = cells.Find(0, Nothing, findOptions)

```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->