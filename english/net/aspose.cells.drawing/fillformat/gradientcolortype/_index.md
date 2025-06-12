---
title: FillFormat.GradientColorType
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Returns the gradient color type for the specified fill
type: docs
url: /net/aspose.cells.drawing/fillformat/gradientcolortype/
---
## FillFormat.GradientColorType property

Returns the gradient color type for the specified fill.

```csharp
public GradientColorType GradientColorType { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Add sample data
            sheet.Cells["A1"].PutValue(50);
            sheet.Cells["A2"].PutValue(100);
            sheet.Cells["A3"].PutValue(150);
            
            // Create chart
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            
            // Set gradient fill for first series
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.SetOneColorGradient(Color.Green, 1, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 1);
            
            // Set two-color gradient for first point
            Aspose.Cells.Charts.ChartPoint point = series.Points[0];
            point.Area.FillFormat.SetTwoColorGradient(Color.Red, Color.Blue, Aspose.Cells.Drawing.GradientStyleType.DiagonalDown, 1);
            
            // Save the workbook
            workbook.Save("GradientColorTypeDemo.xlsx");
        }
    }
}
```

### See Also

* enum [GradientColorType](../../gradientcolortype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


