---
title: "Shape.Worksheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt das Worksheet-Objekt zurück, das diese Form enthält"
type: docs
url: /de/net/aspose.cells.drawing/shape/worksheet/
---
## Shape.Worksheet property

Ruft das [`Worksheet`](../../../aspose.cells/worksheet/) Objekt ab, das diese Form enthält.

```csharp
public Worksheet Worksheet { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Veranschaulichen Sie die Verwendung der Worksheet-Eigenschaft
            Worksheet shapeWorksheet = shape.Worksheet;
            
            // Gib den Worksheet-Namen aus, um zu zeigen, dass die Eigenschaft funktioniert
            Console.WriteLine("Shape belongs to worksheet: " + shapeWorksheet.Name);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


