---
title: "Shape.CreateId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die Erstellungs-ID dieser Form zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/shape/createid/
---
## Shape.CreateId property

Liest und legt die Erstellungs-ID für dieses Shape fest.

```csharp
public Guid CreateId { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyCreateIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 200, 150);
            
            // Erstelle und weise eine neue GUID als CreateId zu
            Guid createId = Guid.NewGuid();
            shape.CreateId = createId;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ShapeCreateIdDemo.xlsx");
            
            // Lade die Arbeitsmappe neu, um zu überprüfen, dass die CreateId erhalten bleibt
            Workbook loadedWorkbook = new Workbook("ShapeCreateIdDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Gib die CreateId zur Verifizierung aus
            Console.WriteLine("Original CreateId: " + createId);
            Console.WriteLine("Loaded CreateId: " + loadedShape.CreateId);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


