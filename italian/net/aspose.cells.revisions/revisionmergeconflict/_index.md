---
title: "Classe RevisionMergeConflict"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Revisions.RevisionMergeConflict. Rappresenta un record di revisione che indica che si è verificato un conflitto di unione"
type: docs
url: /it/net/aspose.cells.revisions/revisionmergeconflict/
---
## RevisionMergeConflict class

Rappresenta un record di revisione che indica che si è verificato un conflitto di merge.

```csharp
public class RevisionMergeConflict : Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione.(Ereditato da [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionmergeconflict/type/) { get; } | Ottiene il tipo di revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro.(Ereditato da [`Revision`](../revision/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionsClassRevisionMergeConflictDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Apporta alcune modifiche per creare la cronologia delle revisioni
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue("Another Value");

            // Salva la cartella di lavoro per generare revisioni
            workbook.Save("RevisionMergeConflictDemo_Before.xlsx");

            // Crea uno scenario di conflitto di unione
            worksheet.Cells["A1"].PutValue("Conflicting Change 1");
            worksheet.Cells["A1"].PutValue("Conflicting Change 2");

            // Ottieni la cronologia delle revisioni (itera direttamente attraverso RevisionLogCollection)
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Trova e dimostra RevisionMergeConflict
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionMergeConflict mergeConflict)
                    {
                        // Dimostrare l'accesso al tipo di revisione
                        RevisionType revisionType = mergeConflict.Type;
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionMergeConflictDemo_After.xlsx");
        }
    }
}
```

### Vedi anche

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


