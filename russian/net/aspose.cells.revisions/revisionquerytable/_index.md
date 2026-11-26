---
title: "Класс RevisionQueryTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Revisions.RevisionQueryTable класс. Представляет ревизию изменения поля таблицы запросов"
type: docs
url: /ru/net/aspose.cells.revisions/revisionquerytable/
---
## RevisionQueryTable class

Представляет ревизию изменения поля запросной таблицы.

```csharp
public class RevisionQueryTable : Revision
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionquerytable/cellarea/) { get; } | Получает расположение затронутой таблицы запросов. |
| [FieldId](../../aspose.cells.revisions/revisionquerytable/fieldid/) { get; } | Получает идентификатор конкретного поля таблицы запросов, которое было удалено. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Получает номер этой ревизии.(Наследовано от [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionquerytable/type/) { get; } | Представляет тип ревизии. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Получает лист.(Наследовано от [`Revision`](../revision/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionQueryTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте примерные данные, чтобы создать контекст для таблицы запросов
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Price";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1.20;

                // Примечание: экземпляры RevisionQueryTable обычно получаются из ревизий книги
                // Это концептуальная демонстрация, поскольку мы не можем напрямую создать экземпляр RevisionQueryTable

                // В реальном сценарии вы бы получили доступ к ревизиям так:
                // RevisionCollection revisions = workbook.Worksheets.Revisions;
                // foreach (Revision revision in revisions)
                // {
                //     if (revision is RevisionQueryTable queryTableRevision)
                //     {
                //         // Доступ к свойствам
                //     }
                // }

                // Для демонстрации мы покажем, как работать со свойствами RevisionQueryTable
                // если бы у нас был экземпляр
                Console.WriteLine("RevisionQueryTable properties demonstration:");
                Console.WriteLine("Type property would return: " + RevisionType.QueryTable);
                Console.WriteLine("FieldId property would return an integer ID of the affected field");
                Console.WriteLine("CellArea property would return the location of the query table");

                // Сохраните книгу
                workbook.Save("RevisionQueryTableDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionQueryTable: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


