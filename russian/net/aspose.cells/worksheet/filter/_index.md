---
title: "Worksheet.Filter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Фильтрует диапазон"
type: docs
url: /ru/net/aspose.cells/worksheet/filter/
---
## Worksheet.Filter method

Фильтрует диапазон.

```csharp
public void Filter(CellArea ca)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | CellArea | Диапазон |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class WorksheetMethodFilterWithCellAreaDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить некоторыми образцовыми данными (включая строку заголовка)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            try
            {
                // Определите диапазон, к которому будет применён фильтр
                CellArea filterArea = new CellArea
                {
                    StartRow = 0,      // Row 1 (zero‑based)
                    StartColumn = 0,   // Column A
                    EndRow = 4,        // Row 5
                    EndColumn = 1      // Column B
                };

                // Примените автофильтр к определённой области
                worksheet.Filter(filterArea);

                // Сохраните книгу, чтобы проверить, что фильтр установлен
                workbook.Save("WorksheetFilterWithCellAreaDemo.xlsx");

                Console.WriteLine("Filter applied successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying filter: {ex.Message}");
            }
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


