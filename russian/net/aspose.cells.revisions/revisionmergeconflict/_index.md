---
title: "Класс RevisionMergeConflict"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Revisions.RevisionMergeConflict. Представляет запись ревизии, указывающую на наличие конфликта слияния"
type: docs
url: /ru/net/aspose.cells.revisions/revisionmergeconflict/
---
## RevisionMergeConflict class

Представляет запись ревизии, указывающую на конфликт слияния.

```csharp
public class RevisionMergeConflict : Revision
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Получает номер этой ревизии.(Наследовано от [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionmergeconflict/type/) { get; } | Получает тип ревизии. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Получает лист.(Наследовано от [`Revision`](../revision/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionsClassRevisionMergeConflictDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Внесите некоторые изменения, чтобы создать историю ревизий
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue("Another Value");

            // Сохраните книгу, чтобы создать ревизии
            workbook.Save("RevisionMergeConflictDemo_Before.xlsx");

            // Создайте сценарий конфликта слияния
            worksheet.Cells["A1"].PutValue("Conflicting Change 1");
            worksheet.Cells["A1"].PutValue("Conflicting Change 2");

            // Получите историю ревизий (итерация напрямую через RevisionLogCollection)
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Найдите и продемонстрируйте RevisionMergeConflict
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionMergeConflict mergeConflict)
                    {
                        // Продемонстрировать доступ к типу ревизии
                        RevisionType revisionType = mergeConflict.Type;
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionMergeConflictDemo_After.xlsx");
        }
    }
}
```

### См. также

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


