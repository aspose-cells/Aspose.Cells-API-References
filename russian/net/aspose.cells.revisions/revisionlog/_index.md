---
title: "Класс RevisionLog"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Revisions.RevisionLog. Представляет журнал ревизий"
type: docs
url: /ru/net/aspose.cells.revisions/revisionlog/
---
## RevisionLog class

Представляет журнал ревизий.

```csharp
public class RevisionLog
```

## Свойства

| Имя | Описание |
| --- | --- |
| [MetadataTable](../../aspose.cells.revisions/revisionlog/metadatatable/) { get; } | Получает таблицу, содержащую метаданные о списке конкретных изменений, произошедших в этой книге. |
| [Revisions](../../aspose.cells.revisions/revisionlog/revisions/) { get; } | Получает все ревизии в этом журнале. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogDemo
    {
        public static void RevisionLogExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Получите доступ к журналам ревизий книги
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Проверьте, есть ли какие-либо журналы ревизий
            if (revisionLogs.Count > 0)
            {
                // Получите доступ к первому журналу ревизий
                RevisionLog revisionLog = revisionLogs[0];

                // Получите доступ к таблице метаданных журнала ревизий
                RevisionHeader metadataTable = revisionLog.MetadataTable;

                // Получите доступ к ревизиям в журнале ревизий
                RevisionCollection revisions = revisionLog.Revisions;

                // Отобразите некоторую информацию о ревизиях
                Console.WriteLine("Number of revisions: " + revisions.Count);
                Console.WriteLine("Metadata Table: " + metadataTable.ToString());
            }
            else
            {
                Console.WriteLine("No revision logs found.");
            }

            // Сохраните книгу
            workbook.Save("RevisionLogExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


