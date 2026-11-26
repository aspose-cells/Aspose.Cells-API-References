---
title: "Класс Revision"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Revisions.Revision класс. Представляет ревизию"
type: docs
url: /ru/net/aspose.cells.revisions/revision/
---
## Revision class

Представляет ревизию.

```csharp
public abstract class Revision
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Получает номер этой ревизии. |
| virtual [Type](../../aspose.cells.revisions/revision/type/) { get; } | Представляет тип ревизии. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Получает лист. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте некоторые данные, чтобы потенциально создать ревизии
                worksheet.Cells["A1"].PutValue("Original Value");

                // Сохраните книгу, чтобы установить базовый уровень
                workbook.Save("RevisionDemo_Baseline.xlsx");

                // Загрузите книгу и внесите изменение
                Workbook modifiedWorkbook = new Workbook("RevisionDemo_Baseline.xlsx");
                modifiedWorkbook.Worksheets[0].Cells["A1"].PutValue("Modified Value");

                // Проверьте, есть ли какие-либо журналы ревизий
                if (modifiedWorkbook.Worksheets.RevisionLogs.Count > 0)
                {
                    RevisionLog log = modifiedWorkbook.Worksheets.RevisionLogs[0];
                    if (log.Revisions.Count > 0)
                    {
                        // Получить первую ревизию
                        Revision revision = log.Revisions[0];

                        // Отобразить свойства только для чтения
                        Console.WriteLine($"Revision ID: {revision.Id}");
                        Console.WriteLine($"Revision Type: {revision.Type}");
                        Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");

                        // Сохранить изменённую книгу
                        modifiedWorkbook.Save("RevisionDemo_Modified.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs available");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with Revision: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


