---
title: "RevisionCellComment.IsOldComment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellComment. Indique s'il s'agit d'un ancien commentaire"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellcomment/isoldcomment/
---
## RevisionCellComment.IsOldComment property

Indique s'il s'agit d'un ancien commentaire.

```csharp
public bool IsOldComment { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyIsOldCommentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec suivi des révisions
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire initial à la cellule A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "First version of comment";

            // Modifier le commentaire pour générer une révision
            comment.Note = "Updated comment text";

            // Ajouter un autre commentaire à la cellule B2
            Comment secondComment = worksheet.Comments[1, 1];
            secondComment.Note = "Second comment";

            // Accédez aux révisions
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Afficher la valeur de la propriété IsOldComment
                    Console.WriteLine("Cell: " + commentRevision.CellName);
                    Console.WriteLine("IsOldComment: " + commentRevision.IsOldComment);
                    
                    // Démontrer l'utilisation de la propriété IsOldComment
                    if (commentRevision.IsOldComment)
                    {
                        Console.WriteLine("This revision represents the old state of the comment");
                        Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    }
                    else
                    {
                        Console.WriteLine("This revision represents the new state of the comment");
                        Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    }

                    // Afficher les propriétés associées
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionCellCommentPropertyIsOldCommentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


