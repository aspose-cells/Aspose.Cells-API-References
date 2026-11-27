---
title: "Shape.GetResultOfSmartArt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Konverterar smart art till grupperade former"
type: docs
url: /sv/net/aspose.cells.drawing/shape/getresultofsmartart/
---
## Shape.GetResultOfSmartArt method

Konverterar smart art till grupperade former.

```csharp
public virtual GroupShape GetResultOfSmartArt()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetResultOfSmartArtDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform (eftersom vi inte kan skapa SmartArt direkt)
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 200, 200, 0, 0);
            
            // I ett verkligt scenario skulle vi ladda en befintlig SmartArt-form
            // För demonstrationsändamål hoppar vi över IsSmartArt-kontrollen eftersom vi inte kan ställa in den

            // Hämta resultatet av SmartArt (fungerar bara om formen faktiskt var SmartArt)
            GroupShape groupShape = shape.GetResultOfSmartArt();
            Console.WriteLine("Converted shape to GroupShape");
        }
    }
}
```

### Se även

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


