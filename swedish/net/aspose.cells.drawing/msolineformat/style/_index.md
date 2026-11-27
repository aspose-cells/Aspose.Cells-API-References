---
title: "MsoLineFormat.Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormat-egenskap. Returnerar ett Style-objekt som representerar stilen för det angivna intervallet"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformat/style/
---
## MsoLineFormat.Style property

Returnerar ett Style-objekt som representerar stilen för det angivna intervallet.

```csharp
public MsoLineStyle Style { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en linjeform
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 150, 10, 10);

            // Hämta linjeformatet
            MsoLineFormat lineFormat = line.LineFormat;

            // Ställ in radstilsegenskaper
            lineFormat.Style = MsoLineStyle.ThickBetweenThin;
            lineFormat.ForeColor = System.Drawing.Color.Red;
            lineFormat.BackColor = System.Drawing.Color.White;
            lineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 3.0;

            // Skapa en annan linje för jämförelse
            Aspose.Cells.Drawing.LineShape line2 = worksheet.Shapes.AddLine(5, 25, 100, 150, 10, 10);
            MsoLineFormat lineFormat2 = line2.LineFormat;

            // Kopiera stil från första linjen till den andra linjen
            lineFormat2.Style = lineFormat.Style;
            lineFormat2.ForeColor = lineFormat.ForeColor;
            lineFormat2.BackColor = lineFormat.BackColor;
            lineFormat2.DashStyle = lineFormat.DashStyle;
            lineFormat2.Transparency = lineFormat.Transparency;
            lineFormat2.Weight = lineFormat.Weight;

            // Spara arbetsboken
            workbook.Save("MsoLineFormatStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


