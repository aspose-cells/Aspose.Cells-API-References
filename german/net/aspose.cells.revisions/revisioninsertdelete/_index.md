---
title: "Klasse RevisionInsertDelete"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionInsertDelete Klasse. Stellt einen Revisionsdatensatz einer Zeilen‑/Spalten‑Einfüge‑/Lösch‑Aktion dar"
type: docs
url: /de/net/aspose.cells.revisions/revisioninsertdelete/
---
## RevisionInsertDelete class

Stellt einen Revisionsdatensatz einer Zeilen-/Spalten-Einfüge-/Löschaktion dar.

```csharp
public class RevisionInsertDelete : Revision
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertdelete/actiontype/) { get; } | Ermittelt den Aktionstyp dieser Revision. |
| [CellArea](../../aspose.cells.revisions/revisioninsertdelete/cellarea/) { get; } | Ermittelt den Einfüge‑/Löschbereich. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ermittelt die Nummer dieser Revision.(Vererbt von [`Revision`](../revision/).) |
| [Revisions](../../aspose.cells.revisions/revisioninsertdelete/revisions/) { get; } | Ermittelt die Revisionsliste für diese Operation. |
| override [Type](../../aspose.cells.revisions/revisioninsertdelete/type/) { get; } | Stellt den Typ der Revision dar. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ermittelt das Arbeitsblatt.(Vererbt von [`Revision`](../revision/).) |

### Beispiele

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

### Siehe auch

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


