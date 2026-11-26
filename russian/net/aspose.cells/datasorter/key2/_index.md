---
title: "DataSorter.Key2"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorter. Представляет индекс второго сортируемого столбца; абсолютная позиция: столбец A — 0, B — 1"
type: docs
url: /ru/net/aspose.cells/datasorter/key2/
---
## DataSorter.Key2 property

Представляет индекс второго отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...).

```csharp
public int Key2 { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey2Demo
    {
        public static void Run()
        {
            // Создайте рабочую книгу и добавьте примерные данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Создать DataSorter и установить свойства
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.Key1 = 0; // Sort by first column (Name)
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key2 = 1; // Then sort by second column (Age)
            sorter.Order2 = SortOrder.Descending;

            // Отсортировать диапазон данных
            sorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Вывести отсортированные данные, чтобы продемонстрировать использование Key2
            Console.WriteLine("Sorted Data:");
            for (int i = 0; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[i, 0].StringValue} - {worksheet.Cells[i, 1].IntValue}");
            }
        }
    }
}
```

### См. также

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


