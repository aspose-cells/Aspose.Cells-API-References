---
title: "ShapeCollection.CopyCommentsInRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Kopiera alla kommentarer i intervallet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/copycommentsinrange/
---
## ShapeCollection.CopyCommentsInRange method

Kopiera alla kommentarer i området.

```csharp
public void CopyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| former | ShapeCollection | Källformerna. |
| ca | CellArea | Det källintervallet. |
| destRow | Int32 | Destinationens startrad för intervallet. |
| destColumn | Int32 | Destinationens startkolumn för intervallet. |

### Exempel

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
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till kommentarer
            CommentCollection comments = worksheet.Comments;
            
            // Lägg till kommentar i cell A1
            int commentIndex = comments.Add(0, 0);
            Comment comment = comments[commentIndex];
            comment.Note = "First note.";
            comment.Font.Name = "Times New Roman";
            
            // Lägg till kommentar i cell B2
            comments.Add("B2");
            comment = comments["B2"];
            comment.Note = "Second note.";
            
            // Definiera källintervall
            CellArea sourceArea = new CellArea();
            sourceArea.StartRow = 0;
            sourceArea.StartColumn = 0;
            sourceArea.EndRow = 1;
            sourceArea.EndColumn = 1;
            
            // Hämta samling av former
            ShapeCollection shapes = worksheet.Shapes;
            
            // Kopiera kommentarer från källintervall till destination (börjar på rad 5, kolumn 1)
            shapes.CopyCommentsInRange(shapes, sourceArea, 5, 1);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


