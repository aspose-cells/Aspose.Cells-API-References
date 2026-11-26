---
title: "RevisionLogCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionLogCollection. Получает RevisionLog по индексу"
type: docs
url: /ru/net/aspose.cells.revisions/revisionlogcollection/item/
---
## RevisionLogCollection indexer

Получает [`RevisionLog`](../../revisionlog/) по индексу.

```csharp
public RevisionLog this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

Возвращает объект [`RevisionLog`](../../revisionlog/).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Включите совместную рабочую книгу, чтобы поддерживать ревизии
            workbook.Settings.Shared = true;

            // Получите доступ к коллекции журналов ревизий
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            try
            {
                // Проверьте, есть ли какие-либо журналы ревизий
                if (revisionLogs.Count > 0)
                {
                    // Получите доступ к первому журналу ревизий, используя свойство Item
                    RevisionLog firstLog = revisionLogs[0];

                    // Отобразите базовую информацию о журнале ревизий
                    Console.WriteLine("First revision log accessed via Item property:");
                    Console.WriteLine($"Revision count: {firstLog.Revisions.Count}");
                }
                else
                {
                    Console.WriteLine("No revision logs available in the workbook.");
                }

                // Сохраните книгу
                workbook.Save("RevisionLogItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [RevisionLog](../../revisionlog/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


