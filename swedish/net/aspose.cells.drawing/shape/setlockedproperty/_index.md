---
title: "Shape.SetLockedProperty"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑metod. Ange den låsta egenskapen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/setlockedproperty/
---
## Shape.SetLockedProperty method

Ställ in den låsta egenskapen.

```csharp
public void SetLockedProperty(ShapeLockType type, bool value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ShapeLockType | Den låsta typen. |
| värde | Boolean | Värdet på egenskapen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLockedPropertyWithShapeLockTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // Demonstrera användning av SetLockedProperty
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);
            shape.SetLockedProperty(ShapeLockType.Selection, false);

            Console.WriteLine("Shape locked properties set successfully.");
        }
    }
}
```

### Se även

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


