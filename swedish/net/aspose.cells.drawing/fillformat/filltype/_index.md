---
title: "FillFormat.FillType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Hämtar och anger fyllningstyp"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/filltype/
---
## FillFormat.FillType property

Hämtar och anger fyllningstyp

```csharp
public FillType FillType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Ange solid fyllning med färg
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Red;

            // Skriv ut fyllningstypen
            Console.WriteLine("Shape fill type: " + shape.Fill.FillType);

            // Byt till gradientfyllning
            shape.Fill.FillType = FillType.Gradient;
            Console.WriteLine("Shape fill type changed to: " + shape.Fill.FillType);

            // Spara arbetsboken
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


