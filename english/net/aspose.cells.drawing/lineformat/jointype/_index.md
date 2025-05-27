---
title: LineFormat.JoinType
second_title: Aspose.Cells for .NET API Reference
description: LineFormat property. Specifies the line join type
type: docs
url: /net/aspose.cells.drawing/lineformat/jointype/
---
## LineFormat.JoinType property

Specifies the line join type.

```csharp
public LineJoinType JoinType { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyJoinTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a line shape
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Set line join type to Round
            line.Line.JoinType = LineJoinType.Round;

            // Save the workbook
            workbook.Save("LineJoinTypeDemo.xlsx");
        }
    }
}
```

### See Also

* enum [LineJoinType](../../linejointype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


