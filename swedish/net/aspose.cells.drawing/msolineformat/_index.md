---
title: "Klass MsoLineFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MsoLineFormat-klass. Representerar linje- och pilspetsformatering"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformat/
---
## MsoLineFormat class

Representerar linje- och pilspetsformat.

```csharp
public class MsoLineFormat
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformat/backcolor/) { get; set; } | Hämtar och anger kantlinjens bakgrundsfärg. |
| [DashStyle](../../aspose.cells.drawing/msolineformat/dashstyle/) { get; set; } | Hämtar eller anger streckstilen för den angivna linjen. |
| [ForeColor](../../aspose.cells.drawing/msolineformat/forecolor/) { get; set; } | Hämtar och anger kantlinjens förgrundsfärg. |
| [IsVisible](../../aspose.cells.drawing/msolineformat/isvisible/) { get; set; } | Anger om objektet är synligt. |
| [Style](../../aspose.cells.drawing/msolineformat/style/) { get; set; } | Returnerar ett Style-objekt som representerar stilen för det angivna intervallet. |
| [Transparency](../../aspose.cells.drawing/msolineformat/transparency/) { get; set; } | Returnerar eller anger graden av transparens för den angivna fyllningen som ett värde från 0,0 (opak) till 1,0 (klar). |
| [Weight](../../aspose.cells.drawing/msolineformat/weight/) { get; set; } | Returnerar eller anger linjens tjocklek i enheter av pt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatDemo
    {
        public static void MsoLineFormatExample()
        {
            // Instansiera en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bågform till kalkylbladet
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Hämta MsoLineFormat-objektet från formen
            MsoLineFormat lineFormat = arcShape.LineFormat;

            // Ställ in egenskaper för MsoLineFormat-objektet
            lineFormat.IsVisible = true;
            lineFormat.Style = MsoLineStyle.ThickThin;
            lineFormat.ForeColor = Color.Red;
            lineFormat.BackColor = Color.Blue;
            lineFormat.DashStyle = MsoLineDashStyle.Solid;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 2.0;

            // Spara arbetsboken
            workbook.Save("MsoLineFormatExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


