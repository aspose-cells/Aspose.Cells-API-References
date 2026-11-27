---
title: "MsoLineFormat.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormat-egenskap. Returnerar eller anger graden av transparens för den angivna fyllningen som ett värde från 0,0 ogenomskinlig till 1,0 klar"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformat/transparency/
---
## MsoLineFormat.Transparency property

Returnerar eller anger graden av transparens för den angivna fyllningen som ett värde från 0,0 (opak) till 1,0 (klar).

```csharp
public double Transparency { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bågform
            ArcShape arc = worksheet.Shapes.AddArc(1, 0, 1, 0, 100, 100);

            // Ange radformatsegenskaper inklusive transparens
            arc.LineFormat.ForeColor = System.Drawing.Color.Red;
            arc.LineFormat.Transparency = 0.5; // 50% transparent
            arc.LineFormat.Weight = 3;
            arc.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Skapa en annan båge för jämförelse
            ArcShape arc2 = worksheet.Shapes.AddArc(1, 2, 1, 2, 100, 100);
            arc2.LineFormat.ForeColor = System.Drawing.Color.Red;
            arc2.LineFormat.Transparency = 0.5; // Same transparency
            arc2.LineFormat.Weight = 3;
            arc2.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Verifiera transparensegenskap
            if (Math.Abs(arc.LineFormat.Transparency - arc2.LineFormat.Transparency) < 0.001)
            {
                Console.WriteLine("Transparency properties match: " + arc.LineFormat.Transparency);
            }
            else
            {
                Console.WriteLine("Transparency properties do not match");
            }

            // Spara arbetsboken
            workbook.Save("MsoLineFormatTransparencyDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


