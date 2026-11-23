---
title: "ShapeCollection.CopyCommentsInRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Copie tous les commentaires dans la plage"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/copycommentsinrange/
---
## ShapeCollection.CopyCommentsInRange method

Copie tous les commentaires dans la plage.

```csharp
public void CopyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formes | ShapeCollection | Les formes source. |
| ca | CellArea | La plage source. |
| destRow | Int32 | La ligne de départ de la plage de destination. |
| destColumn | Int32 | La colonne de départ de la plage de destination. |

### Exemples

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
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des commentaires
            CommentCollection comments = worksheet.Comments;
            
            // Ajouter un commentaire à la cellule A1
            int commentIndex = comments.Add(0, 0);
            Comment comment = comments[commentIndex];
            comment.Note = "First note.";
            comment.Font.Name = "Times New Roman";
            
            // Ajouter un commentaire à la cellule B2
            comments.Add("B2");
            comment = comments["B2"];
            comment.Note = "Second note.";
            
            // Définir la plage source
            CellArea sourceArea = new CellArea();
            sourceArea.StartRow = 0;
            sourceArea.StartColumn = 0;
            sourceArea.EndRow = 1;
            sourceArea.EndColumn = 1;
            
            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;
            
            // Copier les commentaires de la plage source vers la destination (en commençant à la ligne 5, colonne 1)
            shapes.CopyCommentsInRange(shapes, sourceArea, 5, 1);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


