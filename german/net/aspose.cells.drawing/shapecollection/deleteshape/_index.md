---
title: "ShapeCollection.DeleteShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Löschen Sie eine Form. Wenn die Form in der Gruppe ist oder eine Kommentarform ist, wird sie nicht gelöscht."
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/deleteshape/
---
## ShapeCollection.DeleteShape method

Löscht ein Shape. Wenn das Shape in einer Gruppe ist oder ein Kommentar-Shape ist, wird es nicht gelöscht.

```csharp
public void DeleteShape(Shape shape)
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
    public class ShapeCollectionMethodDeleteShapeWithShapeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Formensammlung ab
            ShapeCollection shapes = worksheet.Shapes;

            // Erste Rechteckform hinzufügen
            Shape firstShape = shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Zweite Rechteckform hinzufügen
            Shape secondShape = shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Löschen Sie die erste Form
            shapes.DeleteShape(firstShape);

            // Speichere die Arbeitsmappe
            workbook.Save("DeleteShapeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


