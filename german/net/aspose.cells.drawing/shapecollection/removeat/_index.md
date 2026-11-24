---
title: "ShapeCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Entfernt das Shape"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/removeat/
---
## ShapeCollection.RemoveAt method

Entfernt das Shape.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index des Shape. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodRemoveAtWithInt32Demo
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

            // Entfernt das erste Shape am Index 0
            shapes.RemoveAt(0);

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeCollectionRemoveAtDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


