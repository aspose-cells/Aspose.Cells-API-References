---
title: "Shape.Id"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den Bezeichner dieser Form zurück"
type: docs
url: /de/net/aspose.cells.drawing/shape/id/
---
## Shape.Id property

Liest die Kennung dieses Shapes

```csharp
public int Id { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // ID der Form abrufen und anzeigen
            int id = shape.Id;
            Console.WriteLine("Shape ID: " + id);

            // Eigenschaften der Form ändern
            shape.Name = "Rectangle1";
            shape.Text = "Shape with ID: " + id;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapePropertyIdDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


