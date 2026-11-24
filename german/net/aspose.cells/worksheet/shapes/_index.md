---
title: "Worksheet.Shapes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt alle Zeichenformen in diesem Arbeitsblatt zurück."
type: docs
url: /de/net/aspose.cells/worksheet/shapes/
---
## Worksheet.Shapes property

Gibt alle Zeichenformen in diesem Arbeitsblatt zurück.

```csharp
public ShapeCollection Shapes { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShapesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];
            
            // Füge dem Arbeitsblatt einige Formen hinzu.
            sheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            sheet.Shapes.AddLine(2, 0, 100, 100, 100, 1);
            
            // Formeigenschaften ändern.
            for (int i = 0; i < sheet.Shapes.Count; i++)
            {
                Aspose.Cells.Drawing.Shape shape = sheet.Shapes[i];
                Console.WriteLine($"Shape {i}: Type={shape.Type}, Name={shape.Name}");
                
                // Eigenschaften der ersten Form aktualisieren.
                if (i == 0)
                {
                    shape.Name = "MyRectangle";
                    shape.FillFormat.ForeColor = System.Drawing.Color.Red;
                }
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ShapesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


