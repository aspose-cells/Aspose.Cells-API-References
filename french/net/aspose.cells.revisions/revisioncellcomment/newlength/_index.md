---
title: "RevisionCellComment.NewLength"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellComment. Obtient la longueur du commentaire avant que cette révision ne soit effectuée"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellcomment/newlength/
---
## RevisionCellComment.NewLength property

Obtient la longueur du commentaire avant que cette révision ne soit effectuée.

```csharp
public int NewLength { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyNewLengthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec suivi des révisions
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule F7
            int commentRow = 6;
            int commentCol = 5;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment text";

            // Modifier le commentaire pour générer une révision
            string updatedComment = "This is an updated and longer comment text";
            comment.Note = updatedComment;

            // Accédez aux révisions
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Afficher la valeur de la propriété NewLength
                    Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    Console.WriteLine("Actual new comment length: " + updatedComment.Length);
                    
                    // Affichez les propriétés associées
                    Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    
                    // Démontrer l'utilisation de la propriété NewLength
                    if (commentRevision.NewLength > commentRevision.OldLength)
                    {
                        Console.WriteLine("Comment was expanded by " + 
                            (commentRevision.NewLength - commentRevision.OldLength) + " characters");
                    }
                    else if (commentRevision.NewLength < commentRevision.OldLength)
                    {
                        Console.WriteLine("Comment was shortened by " + 
                            (commentRevision.OldLength - commentRevision.NewLength) + " characters");
                    }
                    else
                    {
                        Console.WriteLine("Comment length remained the same");
                    }
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionCellCommentPropertyNewLengthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


