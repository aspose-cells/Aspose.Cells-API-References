---
title: Class Border
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Border class. Encapsulates the object that represents the cell border
type: docs
url: /net/aspose.cells/border/
---
## Border class

Encapsulates the object that represents the cell border.

```csharp
public class Border
```

## Properties

| Name | Description |
| --- | --- |
| [ArgbColor](../../aspose.cells/border/argbcolor/) { get; set; } | Gets and sets the color with a 32-bit ARGB value. |
| [Color](../../aspose.cells/border/color/) { get; set; } | Gets or sets the Color of the border. |
| [LineStyle](../../aspose.cells/border/linestyle/) { get; set; } | Gets or sets the cell border type. |
| [ThemeColor](../../aspose.cells/border/themecolor/) { get; set; } | Gets and sets the theme color of the border. |

### Examples

```csharp
[C#]
Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;
Cell cell = sheets[0].Cells["A1"];

Style style = cell.GetStyle();
//Set top border style and color
Border border = style.Borders[BorderType.TopBorder];
border.LineStyle = CellBorderType.Medium;
border.Color = Color.Red;
cell.SetStyle(style);

[Visual Basic]
Dim workbook as Workbook  = New Workbook()

Dim sheets as WorksheetCollection  = workbook.Worksheets
Cell cell = sheets(0).Cells("A1");
Dim style as Style = cell.GetStyle()
'Set top border style and color
Dim border as Border = style.Borders(BorderType.TopBorder)
border.LineStyle = CellBorderType.Medium
border.Color = Color.Red
cell.SetStyle(style);
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


