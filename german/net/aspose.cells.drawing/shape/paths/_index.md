---
title: "Shape.Paths"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die Pfade einer benutzerdefinierten geometrischen Form zurück"
type: docs
url: /de/net/aspose.cells.drawing/shape/paths/
---
## Shape.Paths property

Liest die Pfade einer benutzerdefinierten geometrischen Form.

```csharp
public ShapePathCollection Paths { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPathsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine benutzerdefinierte Form (Rechteck) mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 1, 1, 100, 150);

            // Überprüfe, ob die Form benutzerdefinierte Geometriepfade hat
            if (shape.Paths != null)
            {
                Console.WriteLine("Shape has custom geometry paths:");
                Console.WriteLine($"Number of paths: {shape.Paths.Count}");
                
                // Füge der Geometrie der Form einen neuen Pfad hinzu
                int newPathIndex = shape.Paths.Add();
                Console.WriteLine($"Added new path at index: {newPathIndex}");
            }
            else
            {
                Console.WriteLine("No custom geometry path.");
            }
        }
    }
}
```

### Siehe auch

* class [ShapePathCollection](../../shapepathcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


