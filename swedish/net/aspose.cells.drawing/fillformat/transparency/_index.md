---
title: "FillFormat.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Returnerar eller anger transparensgraden för området som ett värde från 0,0 ogenomskinligt till 1,0 helt genomskinligt"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/transparency/
---
## FillFormat.Transparency property

Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar).

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
    public class FillFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera transparens
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 200, 100, 50, 50);

            // Ställ in fyllningsegenskaper med transparens
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            shape.Fill.Transparency = 0.3; // 30% transparent

            // Spara arbetsboken
            workbook.Save("FillFormatTransparencyDemo.xlsx");
        }
    }
}
```

### Se även

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


