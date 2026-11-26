---
title: "Перечисление SortOrder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.SortOrder. Представляет порядок сортировки для диапазона данных"
type: docs
url: /ru/net/aspose.cells/sortorder/
---
## SortOrder enumeration

Представляет порядок сортировки для диапазона данных.

```csharp
public enum SortOrder
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Ascending | `0` | Сортирует данные по возрастанию |
| Descending | `1` | Сортирует данные по убыванию |
| Natural | `2` | Сохраняет исходный порядок данных без сортировки. Применяется только в некоторых специальных сценариях, таких как PivotTable. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSortOrderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            var workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сортировки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);
            
            // Создать сортировщик данных
            var sorter = workbook.DataSorter;
            
            // Установить порядок сортировки и ключи
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Определить область сортировки
            var sortArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };
            
            // Выполните сортировку
            sorter.Sort(worksheet.Cells, sortArea);
            
            // Сохраните книгу
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


