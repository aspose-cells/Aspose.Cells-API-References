---
title: "LineFormat.JoinType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LineFormat egenskap. Anger linjens anslutningstyp"
type: docs
url: /sv/net/aspose.cells.drawing/lineformat/jointype/
---
## LineFormat.JoinType property

Anger linjens anslutningstyp.

```csharp
public LineJoinType JoinType { get; set; }
```

### Exempel

```csharp
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

            // Skapa en linjeform
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Ange linjeanslutningstyp till Rund
            line.Line.JoinType = LineJoinType.Round;

            // Spara arbetsboken
            workbook.Save("LineJoinTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [LineJoinType](../../linejointype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


