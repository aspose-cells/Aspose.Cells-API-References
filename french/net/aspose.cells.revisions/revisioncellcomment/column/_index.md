---
title: "RevisionCellComment.Column"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellComment. Obtient l'index de colonne de celle qui contient un commentaire"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellcomment/column/
---
## RevisionCellComment.Column property

Obtient l'index de la colonne qui contient un commentaire.

```csharp
public int Column { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule D3
            int commentRow = 2;
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
                    
                    // Afficher la valeur de la propriété Column
                    Console.WriteLine("Comment revision column index: " + commentRevision.Column);
                    
                    // Démontrer l'utilisation de la propriété Column
                    Console.WriteLine("Comment was modified in column: " + (char)('A' + commentRevision.Column));
                    
                    // Afficher les propriétés associées
                    Console.WriteLine("Associated row: " + commentRevision.Row);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Remarque : la colonne est en lecture seule, nous ne pouvons donc pas la modifier directement
                    // Nous pouvons la modifier indirectement en modifiant CellName
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "E5"; // This will update both Row and Column properties
                    Console.WriteLine("After CellName change - New column: " + commentRevision.Column);
                    
                    // Restaurer la valeur d'origine
                    commentRevision.CellName = originalCellName;
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionCellCommentPropertyColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


