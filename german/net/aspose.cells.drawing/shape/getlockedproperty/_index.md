---
title: "Shape.GetLockedProperty"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Gibt den Wert der gesperrten Eigenschaft zurück"
type: docs
url: /de/net/aspose.cells.drawing/shape/getlockedproperty/
---
## Shape.GetLockedProperty method

Ermittelt den Wert der gesperrten Eigenschaft.

```csharp
public bool GetLockedProperty(ShapeLockType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ShapeLockType | Der Typ der gesperrten Eigenschaft der Form. |

### Rückgabewert

Gibt den Wert der gesperrten Eigenschaft zurück.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Gesperrte Eigenschaft für AdjustHandles festlegen
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);

            // Prüfen, ob AdjustHandles gesperrt ist
            int noAdjustHandles = 0;
            if (shape.GetLockedProperty(ShapeLockType.AdjustHandles))
                noAdjustHandles = 1;

            Console.WriteLine("AdjustHandles locked status: " + (noAdjustHandles == 1));
        }
    }
}
```

### Siehe auch

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


