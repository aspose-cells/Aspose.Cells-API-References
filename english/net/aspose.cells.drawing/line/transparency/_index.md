---
title: Line.Transparency
second_title: Aspose.Cells for .NET API Reference
description: Line property. Returns or sets the degree of transparency of the line as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/line/transparency/
---
## Line.Transparency property

Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyTransparencyDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a line shape
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 150, 200, 0);

            // Set line properties including transparency
            line.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            line.LineFormat.Weight = 2.5;
            line.LineFormat.ForeColor = Color.Red;
            
            // Set transparency (0 = opaque, 1 = fully transparent)
            line.LineFormat.Transparency = 0.5; // 50% transparent

            // Save the workbook
            workbook.Save("LineTransparencyDemo.xlsx");
        }
    }
}
```

### See Also

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


