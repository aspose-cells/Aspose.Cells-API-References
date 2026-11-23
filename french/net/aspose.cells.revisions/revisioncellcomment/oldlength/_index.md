---
title: "RevisionCellComment.OldLength"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellComment. Obtient la longueur du texte du commentaire ajouté dans cette révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellcomment/oldlength/
---
## RevisionCellComment.OldLength property

Obtient la longueur du texte du commentaire ajouté dans cette révision.

```csharp
public int OldLength { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyOldLengthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec suivi des révisions
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un commentaire à la cellule D4
            int commentRow = 3;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            string initialComment = "Original comment text";
            comment.Note = initialComment;

            // Modifier le commentaire pour générer une révision
            string updatedComment = "This is the modified comment text with more content";
            comment.Note = updatedComment;

            // Accédez aux révisions
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Affichez la valeur de la propriété OldLength
                    Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    Console.WriteLine("Actual initial comment length: " + initialComment.Length);
                    
                    // Affichez les propriétés associées
                    Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    
                    // Démontrez l'utilisation de la propriété OldLength
                    if (commentRevision.OldLength > 0)
                    {
                        Console.WriteLine("Comment existed before modification with length: " + 
                            commentRevision.OldLength);
                            
                        double expansionPercentage = ((double)(commentRevision.NewLength - commentRevision.OldLength) / 
                            commentRevision.OldLength) * 100;
                        Console.WriteLine($"Comment expanded by {expansionPercentage:F2}%");
                    }
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionCellCommentPropertyOldLengthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


