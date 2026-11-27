---
title: "Shape.MsoDrawingType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape egenskap. Hämtar ritningstyp"
type: docs
url: /sv/net/aspose.cells.drawing/shape/msodrawingtype/
---
## Shape.MsoDrawingType property

Hämtar ritningstyp.

```csharp
public MsoDrawingType MsoDrawingType { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMsoDrawingTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform (korrigerade parametrar)
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            
            // Hämta och visa MsoDrawingType för formen
            MsoDrawingType drawingType = rectangle.MsoDrawingType;
            Console.WriteLine("Shape MsoDrawingType: " + drawingType.ToString());

            // Lägg till en linjeform (korrigerade parametrar)
            Shape line = worksheet.Shapes.AddLine(3, 0, 3, 100, 150, 1);
            
            // Hämta och visa MsoDrawingType för linjen
            drawingType = line.MsoDrawingType;
            Console.WriteLine("Line MsoDrawingType: " + drawingType.ToString());
        }
    }
}
```

### Se även

* enum [MsoDrawingType](../../msodrawingtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


