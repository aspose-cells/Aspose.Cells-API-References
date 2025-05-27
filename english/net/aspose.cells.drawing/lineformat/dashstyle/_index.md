---
title: LineFormat.DashStyle
second_title: Aspose.Cells for .NET API Reference
description: LineFormat property. Specifies the line dash type
type: docs
url: /net/aspose.cells.drawing/lineformat/dashstyle/
---
## LineFormat.DashStyle property

Specifies the line dash type.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyDashStyleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a line shape to demonstrate DashStyle
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Set different dash styles for the line
            line.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            line.LineFormat.DashStyle = MsoLineDashStyle.Dash;
            line.LineFormat.DashStyle = MsoLineDashStyle.DashDot;
            line.LineFormat.DashStyle = MsoLineDashStyle.DashDotDot;

            // Save the workbook
            workbook.Save("LineFormatDashStyleDemo.xlsx");
        }
    }
}
```

### See Also

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


