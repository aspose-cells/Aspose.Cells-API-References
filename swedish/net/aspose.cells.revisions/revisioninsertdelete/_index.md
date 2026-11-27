---
title: "Klass RevisionInsertDelete"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionInsertDelete klass. Representerar en revisionspost för en rad-/kolumninfognings-/borttagningsåtgärd"
type: docs
url: /sv/net/aspose.cells.revisions/revisioninsertdelete/
---
## RevisionInsertDelete class

Representerar en revisionspost för en rad-/kolumninfogning/‑borttagningsåtgärd.

```csharp
public class RevisionInsertDelete : Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertdelete/actiontype/) { get; } | Hämtar åtgärdstypen för denna revision. |
| [CellArea](../../aspose.cells.revisions/revisioninsertdelete/cellarea/) { get; } | Hämtar infognings-/borttagningsintervallet. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision.(Arv från [`Revision`](../revision/).) |
| [Revisions](../../aspose.cells.revisions/revisioninsertdelete/revisions/) { get; } | Hämtar revisionslistan för denna operation. |
| override [Type](../../aspose.cells.revisions/revisioninsertdelete/type/) { get; } | Representerar typen av revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet.(Arv från [`Revision`](../revision/).) |

### Exempel

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

### Se även

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


