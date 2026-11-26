---
title: "Класс RevisionFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Revisions.RevisionFormat. Представляет запись ревизии с информацией об изменении форматирования"
type: docs
url: /ru/net/aspose.cells.revisions/revisionformat/
---
## RevisionFormat class

Представляет запись ревизии с информацией об изменении форматирования.

```csharp
public class RevisionFormat : Revision
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Areas](../../aspose.cells.revisions/revisionformat/areas/) { get; } | Диапазон, к которому было применено это форматирование. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Получает номер этой ревизии.(Наследовано от [`Revision`](../revision/).) |
| [Style](../../aspose.cells.revisions/revisionformat/style/) { get; } | Получает применённый стиль. |
| override [Type](../../aspose.cells.revisions/revisionformat/type/) { get; } | Получает тип ревизии. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Получает лист.(Наследовано от [`Revision`](../revision/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionFormatDemo
    {
        public static void Run()
        {
            // Создайте новую книгу в режиме совместного доступа, чтобы включить отслеживание ревизий
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте данные и примените форматирование, чтобы создать ревизию
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("Sample Data");

                // Примените стиль, чтобы создать ревизию форматирования
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                cell.SetStyle(style);

                // Получите доступ к журналам ревизий
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Отобразите свойства ревизии
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);

                            // Отобразить информацию о стиле
                            Style revisionStyle = revisionFormat.Style;
                            Console.WriteLine("Font Name: " + revisionStyle.Font.Name);
                            Console.WriteLine("Font Size: " + revisionStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + revisionStyle.Font.IsBold);
                        }
                    }
                }

                // Сохраните книгу
                workbook.Save("RevisionFormatDemo.xlsx");
                Console.WriteLine("RevisionFormat demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionFormat: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


