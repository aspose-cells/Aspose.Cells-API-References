---
title: "RevisionCellComment.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellComment. Obtient le type de révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellcomment/type/
---
## RevisionCellComment.Type property

Obtient le type de révision.

```csharp
public override RevisionType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentRow = 0;
            int commentCol = 0;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment";

            // Suivre les révisions - modifié pour utiliser la propriété HasRevisions
            // Remarque : Dans une utilisation réelle, vous pourriez devoir activer le suivi par d’autres moyens
            // car HasRevisions est une propriété en lecture seule qui indique si des révisions existent

            // Modifier le commentaire pour générer une révision
            comment.Note = "Modified comment";

            // Accédez aux révisions via la collection RevisionLogs du classeur
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Afficher la valeur de la propriété Type
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    
                    // Démontrer l’utilisation de la propriété Type
                    if (commentRevision.Type == RevisionType.Comment)
                    {
                        Console.WriteLine("This revision is related to a comment change");
                        Console.WriteLine("Comment was modified at row: " + commentRevision.Row + ", column: " + commentRevision.Column);
                        Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                        Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    }
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionCellCommentPropertyTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


