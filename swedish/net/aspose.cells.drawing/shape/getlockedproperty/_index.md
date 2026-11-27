---
title: "Shape.GetLockedProperty"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Hämtar värdet på den låsta egenskapen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/getlockedproperty/
---
## Shape.GetLockedProperty method

Hämtar värdet för den låsta egenskapen.

```csharp
public bool GetLockedProperty(ShapeLockType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ShapeLockType | Typen av den låsta egenskapen för formen. |

### Returvärde

Returnerar värdet på den låsta egenskapen.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLockedPropertyWithShapeLockTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Ställ in låst egenskap för AdjustHandles
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);

            // Kontrollera om AdjustHandles är låst
            int noAdjustHandles = 0;
            if (shape.GetLockedProperty(ShapeLockType.AdjustHandles))
                noAdjustHandles = 1;

            Console.WriteLine("AdjustHandles locked status: " + (noAdjustHandles == 1));
        }
    }
}
```

### Se även

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


