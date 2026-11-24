---
title: "Shape.IsLocked"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Wahr bedeutet, dass das Objekt nicht geändert werden kann, wenn das Blatt geschützt ist. Hinweis: Dieser Wert ist nur sinnvoll, wenn das Arbeitsblatt oder die Objekte im Arbeitsblatt geschützt sind."
type: docs
url: /de/net/aspose.cells.drawing/shape/islocked/
---
## Shape.IsLocked property

True bedeutet, dass das Objekt nicht geändert werden kann, wenn das Blatt geschützt ist. Hinweis: Dieser Wert ist nur sinnvoll, wenn das Arbeitsblatt oder die Objekte im Arbeitsblatt geschützt sind.

```csharp
public bool IsLocked { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Schützen Sie das Arbeitsblatt
            worksheet.Protect(ProtectionType.All);

            // Demonstriere das Sperren/Entsperren der Form.
            Console.WriteLine("Original IsLocked state: " + shape.IsLocked);

            // Entsperre die Form.
            shape.IsLocked = false;
            Console.WriteLine("After unlocking, IsLocked state: " + shape.IsLocked);

            // Sperre die Form.
            shape.IsLocked = true;
            Console.WriteLine("After locking, IsLocked state: " + shape.IsLocked);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


