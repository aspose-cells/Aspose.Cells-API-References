---
title: "Cells.ShowGroupDetail"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Разворачивает сгруппированные строки/столбцы"
type: docs
url: /ru/net/aspose.cells/cells/showgroupdetail/
---
## Cells.ShowGroupDetail method

Разворачивает сгруппированные строки/столбцы.

```csharp
public void ShowGroupDetail(bool isVertical, int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isVertical | Boolean | True, разворачивает сгруппированные строки. |
| индекс | Int32 | Индекс строки/столбца |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodShowGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу и получить доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерные данные в строках 5‑7 (индекс с нуля 4‑6)
            for (int row = 4; row <= 6; row++)
            {
                worksheet.Cells[row, 0].PutValue($"Row {row + 1}");
            }

            // Сгруппировать строки 4‑6 (строки Excel 5‑7) и свернуть их изначально
            worksheet.Cells.GroupRows(4, 6, true);

            try
            {
                // Развернуть сгруппированные строки с помощью ShowGroupDetail (isVertical: false для строк, индекс: 4)
                worksheet.Cells.ShowGroupDetail(false, 4);
                Console.WriteLine("ShowGroupDetail method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShowGroupDetail: {ex.Message}");
            }

            // Сохраните рабочую книгу, чтобы продемонстрировать эффект
            workbook.Save("ShowGroupDetailWithBooleanInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


