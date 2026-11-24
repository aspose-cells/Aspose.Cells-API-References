---
title: "ShapeCollection.CopyInRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Kopiert Formen im Bereich in den Zielbereich."
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/copyinrange/
---
## ShapeCollection.CopyInRange method

Kopiert Shapes im Bereich zum Zielbereich.

```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, 
    bool isContained)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceShapes | ShapeCollection | Quellformen. |
| ca | CellArea | Der Quellbereich. |
| destRow | Int32 | Der Zielzeilenindex des Zielbereichs. |
| destColumn | Int32 | Die Zielspalte des Zielbereichs. |
| isContained | Boolean | Ob nur die Formen kopiert werden, die im Bereich enthalten sind. Wenn true, werden nur die Formen im Bereich kopiert. Andernfalls funktioniert es wie MS Office. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodCopyInRangeWithShapeCollectionCellAreaInt32InDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Formensammlung ab
            ShapeCollection shapes = worksheet.Shapes;

            // Rechteckform hinzufügen
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Definieren Sie den Zellbereich, von dem kopiert werden soll
            CellArea area2 = new CellArea();
            area2.StartColumn = 1;
            area2.StartRow = 1;
            area2.EndColumn = 5;
            area2.EndRow = 11;

            // Formen im angegebenen Bereich kopieren
            shapes.CopyInRange(shapes, area2, 12, 1, false);

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeCopyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


