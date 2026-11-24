---
title: "ShapeCollection.CopyCommentsInRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Kopiert alle Kommentare im Bereich"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/copycommentsinrange/
---
## ShapeCollection.CopyCommentsInRange method

Kopiert alle Kommentare im Bereich.

```csharp
public void CopyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formen | ShapeCollection | Die Quellformen. |
| ca | CellArea | Der Quellbereich. |
| destRow | Int32 | Die Startzeile des Zielbereichs. |
| destColumn | Int32 | Die Startspalte des Zielbereichs. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodCopyCommentsInRangeWithShapeCollectionCellAreaInt32InDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kommentare hinzufügen
            CommentCollection comments = worksheet.Comments;
            
            // Kommentar zu Zelle A1 hinzufügen
            int commentIndex = comments.Add(0, 0);
            Comment comment = comments[commentIndex];
            comment.Note = "First note.";
            comment.Font.Name = "Times New Roman";
            
            // Kommentar zu Zelle B2 hinzufügen
            comments.Add("B2");
            comment = comments["B2"];
            comment.Note = "Second note.";
            
            // Quellbereich definieren
            CellArea sourceArea = new CellArea();
            sourceArea.StartRow = 0;
            sourceArea.StartColumn = 0;
            sourceArea.EndRow = 1;
            sourceArea.EndColumn = 1;
            
            // Formensammlung abrufen
            ShapeCollection shapes = worksheet.Shapes;
            
            // Kommentare vom Quellbereich zum Ziel kopieren (beginnend bei Zeile 5, Spalte 1)
            shapes.CopyCommentsInRange(shapes, sourceArea, 5, 1);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


