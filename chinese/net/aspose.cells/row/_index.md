---
title: Row
second_title: Aspose.Cells for .NET API 参考
description: 表示工作表中的单行
type: docs
weight: 5500
url: /zh/net/aspose.cells/row/
---
## Row class

表示工作表中的单行。

```csharp
public class Row : IEnumerable
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [FirstCell](../../aspose.cells/row/firstcell) { get; } | 获取行中的第一个单元格对象。 |
| [FirstDataCell](../../aspose.cells/row/firstdatacell) { get; } | 获取行中的第一个非空白单元格。 |
| [GroupLevel](../../aspose.cells/row/grouplevel) { get; } | 获取行的组级别。 |
| [Height](../../aspose.cells/row/height) { get; set; } | 以点为单位获取和设置行高。 |
| [Index](../../aspose.cells/row/index) { get; } | 获取该行的索引。 |
| [IsBlank](../../aspose.cells/row/isblank) { get; } | 指示该行是否包含任何数据 |
| [IsCollapsed](../../aspose.cells/row/iscollapsed) { get; set; } | 行是否折叠 |
| [IsHeightMatched](../../aspose.cells/row/isheightmatched) { get; set; } | 表示行高和默认字体高度匹配。 |
| [IsHidden](../../aspose.cells/row/ishidden) { get; set; } | 表示该行是否隐藏。 |
| [Item](../../aspose.cells/row/item) { get; } | 获取单元格。 |
| [LastCell](../../aspose.cells/row/lastcell) { get; } | 获取行中的最后一个单元格对象。 |
| [LastDataCell](../../aspose.cells/row/lastdatacell) { get; } | 获取行中最后一个非空白单元格。 |
| [Style](../../aspose.cells/row/style) { get; } | 表示这一行的样式。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [ApplyStyle](../../aspose.cells/row/applystyle)(Style, StyleFlag) | 对整行应用格式。 |
| [CopySettings](../../aspose.cells/row/copysettings)(Row, bool) | 复制行的设置，例如样式、高度、可见性等。 |
| [Equals](../../aspose.cells/row/equals#equals_1)(object) | 检查此对象是否与另一个对象引用同一行。 |
| [Equals](../../aspose.cells/row/equals#equals)(Row) | 检查此对象是否与另一个行对象引用同一行。 |
| [GetCellOrNull](../../aspose.cells/row/getcellornull)(int) | 获取特定索引中的单元格或 null。 |
| [GetEnumerator](../../aspose.cells/row/getenumerator)() | 获取单元格枚举器 |

### 例子

```csharp

[C#]

 //实例化一个工作簿对象
Workbook workbook = new Workbook();

//获取第一个worksheet

Worksheet worksheet = workbook.Worksheets[0];
Style style = workbook.CreateStyle();

//设置背景颜色为Blue
style.BackgroundColor = Color.Blue;

 //设置前景色为Red
style.ForegroundColor= Color.Red;

 //设置背景图案
style.Pattern = BackgroundType.DiagonalStripe;

 //新样式标志
StyleFlag styleFlag = new StyleFlag();

 //设置所有样式
styleFlag.All = true;

  //获取第一行
Row row = worksheet.Cells.Rows[0];
  //将样式应用到第一行
row.ApplyStyle(style, styleFlag);

 //保存Excel文件
workbook.Save("book1.xls");

[VB.NET]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()

'Obtaining the reference of the first worksheet
Dim worksheet As Worksheet = workbook.Worksheets(0)

Dim style As Style = workbook.CreateStyle()

'Setting the background color to Blue
style.BackgroundColor = Color.Blue

'Setting the foreground color to Red
style.ForegroundColor = Color.Red

'setting Background Pattern
style.Pattern = BackgroundType.DiagonalStripe

'New Style Flag
Dim styleFlag As New StyleFlag()

'Set All Styles
styleFlag.All = True

 'Get first row
Dim row as Row = worksheet.Cells.Rows(0)
 'Apply Style to first row
row.ApplyStyle(style, styleFlag)

'Saving the Excel file
workbook.Save("book1.xls")
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->