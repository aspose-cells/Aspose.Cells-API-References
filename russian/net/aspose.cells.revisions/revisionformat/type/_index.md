---
title: "RevisionFormat.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionFormat. Получает тип ревизии"
type: docs
url: /ru/net/aspose.cells.revisions/revisionformat/type/
---
## RevisionFormat.Type property

Получает тип ревизии.

```csharp
public override RevisionType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Создайте новую книгу в режиме совместного доступа, чтобы включить отслеживание ревизий
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте данные и примените форматирование, чтобы создать ревизию
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");

            // Примените стиль, чтобы создать ревизию форматирования
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);

            try
            {
                // Получите доступ к журналам ревизий
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Отобразите значение свойства Type
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);

                            // Показать дополнительную информацию о ревизии
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);
                        }
                    }
                }

                // Сохраните книгу
                workbook.Save("RevisionFormatTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


