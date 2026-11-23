---
title: "RevisionCellComment.Row"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellComment. Obtient l'indice de ligne de celui qui contient un commentaire"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellcomment/row/
---
## RevisionCellComment.Row property

Obtient l'index de la ligne qui contient un commentaire.

```csharp
public int Row { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec suivi des révisions
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un commentaire à la cellule D4 (ligne 3, colonne 3)
            int commentRow = 3;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Sample comment for revision tracking";

            // Modifier le commentaire pour générer une révision
            comment.Note = "Updated comment text";

            // Accédez aux révisions
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Affichez la valeur de la propriété Row
                    Console.WriteLine("Comment is located at row: " + commentRevision.Row);
                    
                    // Démontrez l'utilisation de la propriété Row
                    Console.WriteLine("Comment location details:");
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Montrez que Row est en lecture seule en essayant de le modifier (cela provoquera une erreur de compilation)
                    // commentRevision.Row = 5; // Cette ligne est commentée car Row est en lecture seule
                    
                    // Méthode alternative pour changer de position en modifiant CellName
                    Console.WriteLine("\nChanging comment position via CellName...");
                    commentRevision.CellName = "F10"; // Changes to row 9, column 5
                    Console.WriteLine("New Row index: " + commentRevision.Row);
                    Console.WriteLine("New Column index: " + commentRevision.Column);
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionCellCommentPropertyRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


