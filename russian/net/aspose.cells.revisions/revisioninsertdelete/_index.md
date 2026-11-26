---
title: "Класс RevisionInsertDelete"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Revisions.RevisionInsertDelete. Представляет запись ревизии действия вставки/удаления строки или столбца"
type: docs
url: /ru/net/aspose.cells.revisions/revisioninsertdelete/
---
## RevisionInsertDelete class

Представляет запись ревизии действия вставки/удаления строки/столбца.

```csharp
public class RevisionInsertDelete : Revision
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertdelete/actiontype/) { get; } | Получает тип действия этой ревизии. |
| [CellArea](../../aspose.cells.revisions/revisioninsertdelete/cellarea/) { get; } | Получает диапазон вставки/удаления. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Получает номер этой ревизии.(Наследовано от [`Revision`](../revision/).) |
| [Revisions](../../aspose.cells.revisions/revisioninsertdelete/revisions/) { get; } | Получает список ревизий по этой операции. |
| override [Type](../../aspose.cells.revisions/revisioninsertdelete/type/) { get; } | Представляет тип ревизии. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Получает лист.(Наследовано от [`Revision`](../revision/).) |

### Примеры

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

### См. также

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


