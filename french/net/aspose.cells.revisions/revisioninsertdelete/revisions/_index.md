---
title: "RevisionInsertDelete.Revisions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionInsertDelete. Obtient la liste des révisions pour cette opération"
type: docs
url: /fr/net/aspose.cells.revisions/revisioninsertdelete/revisions/
---
## RevisionInsertDelete.Revisions property

Obtient la liste des révisions pour cette opération.

```csharp
public RevisionCollection Revisions { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyRevisionsDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et activez le suivi des révisions
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Effectuer des opérations pour générer des révisions
            worksheet.Cells.InsertRows(0, 1);
            worksheet.Cells.DeleteRows(1, 1);

            // Obtenir les journaux de révisions
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Parcourir tous les journaux de révision
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // Accéder à la propriété Revisions (lecture seule)
                        RevisionCollection revisions = revisionInsertDelete.Revisions;

                        // Afficher les informations sur les révisions
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);
                        Console.WriteLine("Action Type: " + revisionInsertDelete.ActionType);
                        Console.WriteLine("Cell Area: " + revisionInsertDelete.CellArea);
                        Console.WriteLine("Number of related revisions: " + revisions.Count);

                        // Démontrer l'utilisation de la collection Revisions
                        foreach (Revision relatedRevision in revisions)
                        {
                            Console.WriteLine(" - Related revision ID: " + relatedRevision.Id);
                            if (relatedRevision is RevisionInsertDelete)
                            {
                                RevisionInsertDelete relatedInsertDelete = (RevisionInsertDelete)relatedRevision;
                                Console.WriteLine("   Action Type: " + relatedInsertDelete.ActionType);
                                Console.WriteLine("   Cell Area: " + relatedInsertDelete.CellArea);
                            }
                        }
                    }
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionInsertDeletePropertyRevisionsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


