---
title: Class Sparkline
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Charts.Sparkline class. A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data
type: docs
url: /net/aspose.cells.charts/sparkline/
---
## Sparkline class

A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.

```csharp
public class Sparkline
```

## Properties

| Name | Description |
| --- | --- |
| [Column](../../aspose.cells.charts/sparkline/column/) { get; } | Gets the column index of the sparkline. |
| [DataRange](../../aspose.cells.charts/sparkline/datarange/) { get; set; } | Represents the data range of the sparkline. |
| [Row](../../aspose.cells.charts/sparkline/row/) { get; } | Gets the row index of the sparkline. |

## Methods

| Name | Description |
| --- | --- |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage)(ImageOrPrintOptions) | Converts a sparkline to an image. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_1)(Stream, ImageOrPrintOptions) | Converts a sparkline to an image. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_2)(string, ImageOrPrintOptions) | Converts a sparkline to an image. |

### Examples

```csharp
[C#]
 Workbook book = new Workbook(); 
 Worksheet sheet = book.Worksheets[0];

 sheet.Cells["A1"].PutValue(5);
 sheet.Cells["B1"].PutValue(2);
 sheet.Cells["C1"].PutValue(1);
 sheet.Cells["D1"].PutValue(3);
 
 // Define the CellArea
 CellArea ca = new CellArea();
 ca.StartColumn = 4;
 ca.EndColumn = 4;
 ca.StartRow = 0;
 ca.EndRow = 0;

 int idx = sheet.SparklineGroups.Add(Aspose.Cells.Charts.SparklineType.Line, sheet.Name + "!A1:D1", false, ca);

 SparklineGroup group = sheet.SparklineGroups[idx];
 idx = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
 Sparkline line = group.Sparklines[idx];
 Console.WriteLine("Saprkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);
 line.ToImage("output.png", new ImageOrPrintOptions());
```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


