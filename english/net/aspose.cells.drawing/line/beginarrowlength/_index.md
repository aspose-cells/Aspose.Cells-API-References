---
title: Line.BeginArrowLength
second_title: Aspose.Cells for .NET API Reference
description: Line property. Specifies the length of the arrowhead for the begin of a line
type: docs
url: /net/aspose.cells.drawing/line/beginarrowlength/
---
## Line.BeginArrowLength property

Specifies the length of the arrowhead for the begin of a line.

```csharp
public MsoArrowheadLength BeginArrowLength { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyBeginArrowLengthDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a line shape to the worksheet
            LineShape lineShape = worksheet.Shapes.AddLine(5, 5, 100, 150, 5, 5);
            
            // Get the line format properties
            LineFormat lineFormat = lineShape.Line;

            // Set the arrowhead properties
            lineFormat.BeginArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineFormat.BeginArrowheadLength = MsoArrowheadLength.Medium;
            lineFormat.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
            lineFormat.EndArrowheadLength = MsoArrowheadLength.Long;

            // Output the arrowhead length
            Console.WriteLine("Begin Arrowhead Length: " + lineFormat.BeginArrowheadLength);

            // Save the workbook
            workbook.Save("LineArrowLengthDemo.xlsx");
        }
    }
}
```

### See Also

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


