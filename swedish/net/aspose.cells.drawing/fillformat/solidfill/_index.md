---
title: "FillFormat.SolidFill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Hämtar SolidFill-objekt"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/solidfill/
---
## FillFormat.SolidFill property

Hämtar `SolidFill`-objekt.

```csharp
public SolidFill SolidFill { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertySolidFillDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Ställ in solid fyllningsfärg för formen
            shape.Fill.SolidFill.Color = System.Drawing.Color.FromArgb(135, 222, 255);
            
            // Hämta och visa solid fyllningsfärg
            System.Drawing.Color fillColor = shape.Fill.SolidFill.Color;
            Console.WriteLine("Solid Fill Color - R:{0}, G:{1}, B:{2}", 
                fillColor.R, fillColor.G, fillColor.B);
            
            // Spara arbetsboken
            workbook.Save("SolidFillDemo.xlsx");
        }
    }
}
```

### Se även

* class [SolidFill](../../solidfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


