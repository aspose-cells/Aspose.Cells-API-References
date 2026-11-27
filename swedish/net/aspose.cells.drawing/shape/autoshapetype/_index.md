---
title: "Shape.AutoShapeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Hämtar och anger den automatiska formtypen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/autoshapetype/
---
## Shape.AutoShapeType property

Hämtar och anger autotypen för formen.

```csharp
public AutoShapeType AutoShapeType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAutoShapeTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet med korrekta parametrar
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Kontrollera och ändra AutoShapeType om det behövs
            if (shape.AutoShapeType == AutoShapeType.Unknown)
            {
                shape.AutoShapeType = AutoShapeType.Rectangle;
            }

            // Ändra formtypen för att demonstrera egenskapen
            shape.AutoShapeType = AutoShapeType.Oval;

            // Spara arbetsboken
            workbook.Save("ShapePropertyAutoShapeTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


