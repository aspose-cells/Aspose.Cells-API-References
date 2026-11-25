---
title: "Classe RevisionInsertDelete"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Revisions.RevisionInsertDelete. Rappresenta un record di revisione di un'azione di inserimento/eliminazione di riga/colonna"
type: docs
url: /it/net/aspose.cells.revisions/revisioninsertdelete/
---
## RevisionInsertDelete class

Rappresenta un record di revisione di un'azione di inserimento/cancellazione di riga/colonna.

```csharp
public class RevisionInsertDelete : Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertdelete/actiontype/) { get; } | Ottiene il tipo di azione di questa revisione. |
| [CellArea](../../aspose.cells.revisions/revisioninsertdelete/cellarea/) { get; } | Ottiene l'intervallo di inserimento/eliminazione. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione.(Ereditato da [`Revision`](../revision/).) |
| [Revisions](../../aspose.cells.revisions/revisioninsertdelete/revisions/) { get; } | Ottiene l'elenco delle revisioni per questa operazione. |
| override [Type](../../aspose.cells.revisions/revisioninsertdelete/type/) { get; } | Rappresenta il tipo di revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro.(Ereditato da [`Revision`](../revision/).) |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionsClassRevisionInsertDeleteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.InsertRow(0);
            worksheet.Cells.DeleteColumn(0);

            string filePath = "RevisionsDemo.xlsx";
            workbook.Save(filePath);

            Workbook reopenedWorkbook = new Workbook(filePath);
            foreach (RevisionLog log in reopenedWorkbook.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.InsertDelete)
                    {
                        RevisionInsertDelete rid = (RevisionInsertDelete)revision;
                        Console.WriteLine($"ActionType: {rid.ActionType}, CellArea: {rid.CellArea}");
                    }
                }
            }
        }
    }
}
```

### Vedi anche

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


