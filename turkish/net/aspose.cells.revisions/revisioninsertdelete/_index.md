---
title: "Sınıf RevisionInsertDelete"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionInsertDelete sınıfı. Satır/sütun ekleme/silme eyleminin bir revizyon kaydını temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisioninsertdelete/
---
## RevisionInsertDelete class

Satır/sütun ekleme/silme eyleminin bir revizyon kaydını temsil eder.

```csharp
public class RevisionInsertDelete : Revision
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertdelete/actiontype/) { get; } | Bu revizyonun eylem tipini alır. |
| [CellArea](../../aspose.cells.revisions/revisioninsertdelete/cellarea/) { get; } | Ekleme/silme aralığını alır. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Bu revizyonun numarasını alır.(Inherited from [`Revision`](../revision/).) |
| [Revisions](../../aspose.cells.revisions/revisioninsertdelete/revisions/) { get; } | Bu işlemle ilgili revizyon listesini alır. |
| override [Type](../../aspose.cells.revisions/revisioninsertdelete/type/) { get; } | Revizyonun türünü temsil eder. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Çalışma sayfasını alır. ([`Revision`](../revision/) üzerinden devralınmıştır.) |

### Örnekler

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

### Ayrıca Bakınız

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


