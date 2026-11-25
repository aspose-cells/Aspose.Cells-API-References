---
title: "ShapeCollection.CopyCommentsInRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Copia tutti i commenti nell'intervallo"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/copycommentsinrange/
---
## ShapeCollection.CopyCommentsInRange method

Copia tutti i commenti nell'intervallo.

```csharp
public void CopyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| forme | ShapeCollection | Le forme di origine. |
| ca | CellArea | L'intervallo di origine. |
| destRow | Int32 | La riga di inizio dell'intervallo di destinazione. |
| destColumn | Int32 | La colonna di inizio dell'intervallo di destinazione. |

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi commenti
            CommentCollection comments = worksheet.Comments;
            
            // Aggiungi commento alla cella A1
            int commentIndex = comments.Add(0, 0);
            Comment comment = comments[commentIndex];
            comment.Note = "First note.";
            comment.Font.Name = "Times New Roman";
            
            // Aggiungi commento alla cella B2
            comments.Add("B2");
            comment = comments["B2"];
            comment.Note = "Second note.";
            
            // Definisci intervallo di origine
            CellArea sourceArea = new CellArea();
            sourceArea.StartRow = 0;
            sourceArea.StartColumn = 0;
            sourceArea.EndRow = 1;
            sourceArea.EndColumn = 1;
            
            // Ottieni collezione di forme
            ShapeCollection shapes = worksheet.Shapes;
            
            // Copia i commenti dall'intervallo di origine a quello di destinazione (inizio alla riga 5, colonna 1)
            shapes.CopyCommentsInRange(shapes, sourceArea, 5, 1);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


