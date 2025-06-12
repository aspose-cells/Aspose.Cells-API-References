---
title: Line.EndArrowLength
second_title: Aspose.Cells for .NET API Reference
description: Line property. Specifies the length of the arrowhead for the end of a line
type: docs
url: /net/aspose.cells.drawing/line/endarrowlength/
---
## Line.EndArrowLength property

Specifies the length of the arrowhead for the end of a line.

```csharp
public MsoArrowheadLength EndArrowLength { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyEndArrowLengthDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a line shape to the worksheet
            LineShape lineShape = worksheet.Shapes.AddLine(1, 0, 1, 100, 100, 100);
            LineFormat lineFormat = lineShape.Line;

            // Set line properties with arrowheads
            lineFormat.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineFormat.EndArrowheadLength = MsoArrowheadLength.Long;

            // Output the end arrow length
            Console.WriteLine("End Arrowhead Length: " + lineFormat.EndArrowheadLength);

            // Save the workbook
            workbook.Save("LineEndArrowLengthDemo.xlsx");
        }
    }
}
```

### See Also

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


