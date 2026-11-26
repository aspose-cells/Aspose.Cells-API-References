---
title: "FilterColumn.Top10Filter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FilterColumn. Получает Top10Filter для фильтрации данных по их рангу"
type: docs
url: /ru/net/aspose.cells/filtercolumn/top10filter/
---
## FilterColumn.Top10Filter property

Получает `Top10Filter` для фильтрации данных по их рангу.

```csharp
public Top10Filter Top10Filter { get; }
```

### Примечания

Перед использованием этого свойства, пожалуйста, убедитесь, что [`FilterType`](../filtertype/) установлен в Top10, иначе будет возвращено null.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyTop10FilterDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте новую книгу и получите первый лист
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Заполните некоторыми образцовыми данными
                sheet.Cells["A1"].PutValue("Values");
                sheet.Cells["A2"].PutValue(10);
                sheet.Cells["A3"].PutValue(20);
                sheet.Cells["A4"].PutValue(30);
                sheet.Cells["A5"].PutValue(40);

                // Примените AutoFilter к диапазону данных
                sheet.AutoFilter.Range = "A1:A5";

                // Получите первый столбец фильтра (индекс столбца 0)
                FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

                // Отобразите текущий объект Filter (может быть null)
                Console.WriteLine("Current Filter object type: " +
                    (filterColumn.Filter != null ? filterColumn.Filter.GetType().FullName : "null"));

                // Проверьте, является ли применённый фильтр Top10Filter
                if (filterColumn.Filter != null && filterColumn.Filter.GetType().Name == "Top10Filter")
                {
                    Console.WriteLine("The filter column contains a Top10Filter.");
                }
                else
                {
                    Console.WriteLine("No Top10Filter is applied to this column.");
                }

                // Сохраните книгу (необязательно)
                workbook.Save("Top10FilterDemo.xlsx");
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

* class [Top10Filter](../../top10filter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


