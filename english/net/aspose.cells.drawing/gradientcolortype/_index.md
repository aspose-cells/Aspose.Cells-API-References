---
title: Enum GradientColorType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.GradientColorType enum. Represents the gradient color type for the specified fill
type: docs
url: /net/aspose.cells.drawing/gradientcolortype/
---
## GradientColorType enumeration

Represents the gradient color type for the specified fill.

```csharp
public enum GradientColorType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No gradient color |
| OneColor | `1` | One gradient color |
| PresetColors | `2` | Preset gradient colors |
| TwoColors | `3` | Two gradient colors |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassGradientColorTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add sample data for chart
            sheet.Cells["A1"].PutValue(50);
            sheet.Cells["A2"].PutValue(100);
            sheet.Cells["A3"].PutValue(150);

            // Add a chart
            int chartIndex = sheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = sheet.Charts[0];

            // Set chart data range
            chart.NSeries.Add("A1:A3", true);

            // Get first point in first series
            ChartPoint point = chart.NSeries[0].Points[0];

            // Set gradient fill with preset colors
            point.Area.FillFormat.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);
            
            // Save the workbook
            workbook.Save("GradientColorTypeDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


