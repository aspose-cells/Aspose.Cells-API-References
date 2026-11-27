---
title: "Shape.TextShapeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape egenskap. Hämtar och anger den förinställda textformstypen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/textshapetype/
---
## Shape.TextShapeType property

Hämtar och anger den förinställda textformstypen.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Kontrollera och ställ in TextShapeType om den är okänd
            if (shape.TextShapeType == AutoShapeType.Unknown)
            {
                shape.TextShapeType = AutoShapeType.Rectangle;
            }

            // Skriv ut formens TextShapeType
            Console.WriteLine("Shape TextShapeType: " + shape.TextShapeType);
        }
    }
}
```

### Se även

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


