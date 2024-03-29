---
title: Class Column
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Column class. Represents a single column in a worksheet
type: docs
url: /net/aspose.cells/column/
---
## Column class

Represents a single column in a worksheet.

```csharp
public class Column
```

## Properties

| Name | Description |
| --- | --- |
| [GroupLevel](../../aspose.cells/column/grouplevel/) { get; set; } | Gets the group level of the column. |
| [HasCustomStyle](../../aspose.cells/column/hascustomstyle/) { get; } | Indicates whether this column has custom style settings(different from the default one inherited from workbook). |
| [Index](../../aspose.cells/column/index/) { get; } | Gets the index of this column. |
| [IsCollapsed](../../aspose.cells/column/iscollapsed/) { get; set; } | whether the column is collapsed |
| [IsHidden](../../aspose.cells/column/ishidden/) { get; set; } | Indicates whether the column is hidden. |
| [Style](../../aspose.cells/column/style/) { get; } | (**Obsolete.**) Gets the style of this column. |
| [Width](../../aspose.cells/column/width/) { get; set; } | Gets and sets the column width in unit of characters. |

## Methods

| Name | Description |
| --- | --- |
| [ApplyStyle](../../aspose.cells/column/applystyle/)(Style, StyleFlag) | Applies formats for a whole column. |
| [GetStyle](../../aspose.cells/column/getstyle/)() | Gets the style of this column. |
| [SetStyle](../../aspose.cells/column/setstyle/)(Style) | Sets the style of this column. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();

//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Style style = workbook.CreateStyle();

//Setting the background color to Blue
style.BackgroundColor = Color.Blue;

//Setting the foreground color to Red
style.ForegroundColor= Color.Red;

//setting Background Pattern
style.Pattern = BackgroundType.DiagonalStripe;

//New Style Flag
StyleFlag styleFlag = new StyleFlag();

//Set All Styles
styleFlag.All = true;

//Get first Column
Column column = worksheet.Cells.Columns[0];

//Apply Style to first Column
column.ApplyStyle(style, styleFlag);

//Saving the Excel file
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

'Get first Column
Dim column As Column = worksheet.Cells.Columns(0)

'Apply Style to first Column
column.ApplyStyle(style, styleFlag)

'Saving the Excel file
workbook.Save("book1.xls")
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


