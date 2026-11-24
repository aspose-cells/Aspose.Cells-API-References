---
title: "ShapeCollection.Remove"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Entfernt das Shape"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/remove/
---
## ShapeCollection.Remove method

Entfernt das Shape.

```csharp
public void Remove(Shape shape)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Form | Form |  |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodRemoveWithShapeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Formensammlung ab
            ShapeCollection shapes = worksheet.Shapes;

            // Erste Rechteckform hinzufügen
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            // Zweite Rechteckform hinzufügen
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Erhalte die erste Form nach Name oder Index
            Shape shapeToRemove = shapes["Rectangle 1"]; // or shapes[0];
            
            if (shapeToRemove != null)
            {
                // Entferne die Form aus der Sammlung
                shapes.Remove(shapeToRemove);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeRemoveDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


