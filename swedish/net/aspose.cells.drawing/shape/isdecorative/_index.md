---
title: "Shape.IsDecorative"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape egenskap. Anger om objektet är dekorativt"
type: docs
url: /sv/net/aspose.cells.drawing/shape/isdecorative/
---
## Shape.IsDecorative property

Anger om objektet är dekorativt.

```csharp
public bool IsDecorative { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsDecorativeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            
            // Ställ in formen som dekorativ
            shape.IsDecorative = true;
            
            // Spara arbetsboken
            string outputPath = "ShapeIsDecorativeDemo.xlsx";
            workbook.Save(outputPath);
            
            // Läs in arbetsboken igen för att verifiera egenskapen
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Skriv ut resultatet
            Console.WriteLine("Shape IsDecorative property: " + loadedShape.IsDecorative);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


