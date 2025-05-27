---
title: LineFormat.Weight
second_title: Aspose.Cells for .NET API Reference
description: LineFormat property. Gets or sets the weight of the line in unit of points
type: docs
url: /net/aspose.cells.drawing/lineformat/weight/
---
## LineFormat.Weight property

Gets or sets the weight of the line in unit of points.

```csharp
public double Weight { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyWeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a line shape
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 200, 0);

            // Set the line weight
            line.LineFormat.Weight = 2.0d;

            // Save the workbook
            workbook.Save("LineFormatWeightDemo.xlsx");
        }
    }
}
```

### See Also

* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


