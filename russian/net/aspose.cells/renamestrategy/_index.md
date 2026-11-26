---
title: "Перечисление RenameStrategy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.RenameStrategy. Параметр стратегии для дублирующихся имён столбцов"
type: docs
url: /ru/net/aspose.cells/renamestrategy/
---
## RenameStrategy enumeration

Опция стратегии для дублирования имён столбцов.

```csharp
public enum RenameStrategy
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Exception | `0` | Выбрасывает исключение. |
| Digit | `1` | Названо цифрой. Дублированные имена будут выглядеть ...1, ...2 и т.д. |
| Letter | `2` | Названо буквой.. Дублированные имена будут выглядеть ...A, ...B и т.д. |

### Примечания

При обработке данных с заголовками в некоторых сценариях требуется, чтобы заголовки не дублировались во всех столбцах. Например, при экспорте данных в DataTable и необходимости использовать заголовок в качестве имени столбца DataTable, дублирующиеся значения заголовка недопустимы. В подобных ситуациях пользователь может определить, как их обрабатывать, указав эту стратегию.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RenameStrategyDemo
    {
        public static void RenameStrategyExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые образцы данных в лист
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("John");

            // Создайте ExportTableOptions и задайте RenameStrategy
            ExportTableOptions options = new ExportTableOptions
            {
                RenameStrategy = RenameStrategy.Digit // Use the Digit strategy for duplicate names
            };

            // Экспортировать данные листа в DataTable
            System.Data.DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 1, options);

            // Отобразить содержимое DataTable
            foreach (System.Data.DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Сохраните книгу
            workbook.Save("RenameStrategyExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


