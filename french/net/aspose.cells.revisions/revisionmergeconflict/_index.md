---
title: "Classe RevisionMergeConflict"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Revisions.RevisionMergeConflict. Représente un enregistrement de révision indiquant qu'il y a eu un conflit de fusion"
type: docs
url: /fr/net/aspose.cells.revisions/revisionmergeconflict/
---
## RevisionMergeConflict class

Représente un enregistrement de révision indiquant qu'il y a eu un conflit de fusion.

```csharp
public class RevisionMergeConflict : Revision
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtient le numéro de cette révision.(Hérité de [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionmergeconflict/type/) { get; } | Obtient le type de révision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtient la feuille de calcul. (Hérité de [`Revision`](../revision/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionsClassRevisionMergeConflictDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Apportez quelques modifications pour créer l'historique des révisions
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue("Another Value");

            // Enregistrez le classeur pour générer des révisions
            workbook.Save("RevisionMergeConflictDemo_Before.xlsx");

            // Créez un scénario de conflit de fusion
            worksheet.Cells["A1"].PutValue("Conflicting Change 1");
            worksheet.Cells["A1"].PutValue("Conflicting Change 2");

            // Obtenez l'historique des révisions (parcourez directement RevisionLogCollection)
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Trouvez et démontrez RevisionMergeConflict
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionMergeConflict mergeConflict)
                    {
                        // Démontrer l'accès au type de révision
                        RevisionType revisionType = mergeConflict.Type;
                    }
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionMergeConflictDemo_After.xlsx");
        }
    }
}
```

### Voir aussi

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


