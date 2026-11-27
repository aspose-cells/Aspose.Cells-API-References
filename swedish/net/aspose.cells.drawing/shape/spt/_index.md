---
title: "Shape.Spt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Anger ett valfritt nummer som ett program kan använda för att associera den specifika formen med en definierad formtyp"
type: docs
url: /sv/net/aspose.cells.drawing/shape/spt/
---
## Shape.Spt property

Anger ett valfritt nummer som ett program kan använda för att associera den specifika formen med en definierad formtyp.

```csharp
public int Spt { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySptDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 100, 100, 100, 100);

            // Hämta och visa Spt-egenskapen
            int spt = shape.Spt;
            Console.WriteLine("Shape Spt value: " + spt);

            // Skapa en ny oval form för att demonstrera olika Spt-värden
            Shape ovalShape = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 1, 1, 100, 100, 100, 100);
            Console.WriteLine("Oval shape Spt value: " + ovalShape.Spt);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


