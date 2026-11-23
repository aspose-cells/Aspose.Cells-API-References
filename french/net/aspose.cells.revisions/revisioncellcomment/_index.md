---
title: "Classe RevisionCellComment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Revisions.RevisionCellComment. Représente un enregistrement de révision d'une modification de commentaire de cellule"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellcomment/
---
## RevisionCellComment class

Représente un enregistrement de révision d'une modification de commentaire de cellule.

```csharp
public class RevisionCellComment : Revision
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncellcomment/actiontype/) { get; } | Obtient le type d'action de la révision. |
| [CellName](../../aspose.cells.revisions/revisioncellcomment/cellname/) { get; set; } | Obtient le nom de la cellule. |
| [Column](../../aspose.cells.revisions/revisioncellcomment/column/) { get; } | Obtient l'index de la colonne qui contient un commentaire. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtient le numéro de cette révision.(Hérité de [`Revision`](../revision/).) |
| [IsOldComment](../../aspose.cells.revisions/revisioncellcomment/isoldcomment/) { get; } | Indique s'il s'agit d'un ancien commentaire. |
| [NewLength](../../aspose.cells.revisions/revisioncellcomment/newlength/) { get; } | Obtient la longueur du commentaire avant que cette révision ne soit effectuée. |
| [OldLength](../../aspose.cells.revisions/revisioncellcomment/oldlength/) { get; } | Obtient la longueur du texte du commentaire ajouté dans cette révision. |
| [Row](../../aspose.cells.revisions/revisioncellcomment/row/) { get; } | Obtient l'index de la ligne qui contient un commentaire. |
| override [Type](../../aspose.cells.revisions/revisioncellcomment/type/) { get; } | Obtient le type de révision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtient la feuille de calcul. (Hérité de [`Revision`](../revision/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCellCommentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec suivi des révisions
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire initial à la cellule A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment text";

            // Modifier le commentaire pour générer une révision
            comment.Note = "Updated comment with more text";

            // Accéder au journal des révisions
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;

                    // Afficher les propriétés de la révision
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("Row: " + commentRevision.Row);
                    Console.WriteLine("Column: " + commentRevision.Column);

                    // Afficher les changements de longueur du commentaire
                    Console.WriteLine("Old Length: " + commentRevision.OldLength);
                    Console.WriteLine("New Length: " + commentRevision.NewLength);
                    Console.WriteLine("Is Old Comment: " + commentRevision.IsOldComment);

                    // Modifier le nom de la cellule pour démontrer le changement de propriété
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "B2";
                    Console.WriteLine("Modified Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("New Row: " + commentRevision.Row);
                    Console.WriteLine("New Column: " + commentRevision.Column);

                    // Restaurer le nom original de la cellule
                    commentRevision.CellName = originalCellName;
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionsClassRevisionCellCommentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


