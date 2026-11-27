---
title: "LineFormat.CompoundType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LineFormat-egenskap. Anger linjens sammansättningstyp"
type: docs
url: /sv/net/aspose.cells.drawing/lineformat/compoundtype/
---
## LineFormat.CompoundType property

Anger linjens sammansättningstyp.

```csharp
public MsoLineStyle CompoundType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCompoundTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en linjeform
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Hämta linjeformatet
            LineFormat lineFmt = line.Line;

            // Ange sammansatt typ
            lineFmt.CompoundType = MsoLineStyle.Single;

            // Spara arbetsboken
            workbook.Save("LineFormatCompoundTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MsoLineStyle](../../msolinestyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


