---
title: "Shape.SetLockedProperty"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Setzen Sie die gesperrte Eigenschaft"
type: docs
url: /de/net/aspose.cells.drawing/shape/setlockedproperty/
---
## Shape.SetLockedProperty method

Setzt die gesperrte Eigenschaft.

```csharp
public void SetLockedProperty(ShapeLockType type, bool value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ShapeLockType | Der gesperrte Typ. |
| Wert | Boolean | Der Wert der Eigenschaft. |

### Beispiele

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

            // Beispielhafte Form mit allen erforderlichen Parametern hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // Demonstrieren Sie die Verwendung von SetLockedProperty
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);
            shape.SetLockedProperty(ShapeLockType.Selection, false);

            Console.WriteLine("Shape locked properties set successfully.");
        }
    }
}
```

### Siehe auch

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


