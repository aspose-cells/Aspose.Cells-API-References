---
title: "LineFormat.JoinType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LineFormat-Eigenschaft. Gibt den Linienverbindungstyp an."
type: docs
url: /de/net/aspose.cells.drawing/lineformat/jointype/
---
## LineFormat.JoinType property

Gibt den Linienverbindungstyp an.

```csharp
public LineJoinType JoinType { get; set; }
```

### Beispiele

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

            // Erstelle ein Linienobjekt
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Lege den Linienverbindungstyp auf Rund fest
            line.Line.JoinType = LineJoinType.Round;

            // Speichere die Arbeitsmappe
            workbook.Save("LineJoinTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [LineJoinType](../../linejointype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


