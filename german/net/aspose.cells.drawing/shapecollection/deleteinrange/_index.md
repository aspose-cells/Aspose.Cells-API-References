---
title: "ShapeCollection.DeleteInRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Löscht Formen im Bereich. Kommentarformen werden nicht gelöscht"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/deleteinrange/
---
## ShapeCollection.DeleteInRange method

Löscht Shapes im Bereich. Kommentar-Shapes werden nicht gelöscht.

```csharp
public void DeleteInRange(CellArea ca)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | CellArea | Der Bereich.Wenn die Formen im Bereich enthalten sind, werden sie entfernt. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodDeleteInRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Erste Rechteckform hinzufügen
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            // Zweite Rechteckform hinzufügen
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Definiere den Bereich, in dem Formen gelöscht werden sollen
            CellArea area = new CellArea();
            area.StartColumn = 0;
            area.StartRow = 5;
            area.EndColumn = 5;
            area.EndRow = 8;

            // Lösche Formen innerhalb des angegebenen Bereichs
            shapes.DeleteInRange(area);

            // Arbeitsmappe speichern (optional)
            workbook.Save("ShapeDeleteInRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


