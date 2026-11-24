---
title: "Shape.ZOrderPosition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die Position einer Form in der Z‑Reihenfolge zurück"
type: docs
url: /de/net/aspose.cells.drawing/shape/zorderposition/
---
## Shape.ZOrderPosition property

Gibt die Position einer Form in der Z‑Reihenfolge zurück.

```csharp
public int ZOrderPosition { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyZOrderPositionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Drei Formen hinzufügen, um ZOrder zu demonstrieren
            Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);
            Shape shape3 = worksheet.Shapes.AddRectangle(90, 90, 100, 100, 0, 0);

            // ZOrder-Positionen festlegen
            shape1.ZOrderPosition = 0;
            shape2.ZOrderPosition = 1;
            shape3.ZOrderPosition = 2;

            // ZOrder von shape3 ändern, um sie in den Vordergrund zu bringen
            shape3.ZOrderPosition = 0;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeZOrderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


