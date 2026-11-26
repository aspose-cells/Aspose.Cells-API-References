---
title: "DataSorter.Order3"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorter. Представляет порядок сортировки третьего ключа"
type: docs
url: /ru/net/aspose.cells/datasorter/order3/
---
## DataSorter.Order3 property

Представляет порядок сортировки третьего ключа.

```csharp
public SortOrder Order3 { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyOrder3Demo
    {
        public static void Run()
        {
            // Создайте рабочую книгу и добавьте примерные данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные для сортировки
            cells["A1"].PutValue("Department");
            cells["B1"].PutValue("Name");
            cells["C1"].PutValue("Salary");
            
            cells["A2"].PutValue("HR");
            cells["B2"].PutValue("John");
            cells["C2"].PutValue(5000);
            
            cells["A3"].PutValue("IT");
            cells["B3"].PutValue("Alice");
            cells["C3"].PutValue(6000);
            
            cells["A4"].PutValue("HR");
            cells["B4"].PutValue("Bob");
            cells["C4"].PutValue(4500);
            
            cells["A5"].PutValue("IT");
            cells["B5"].PutValue("Charlie");
            cells["C5"].PutValue(7000);

            // Создайте сортировщик данных и задайте ключи и порядок сортировки
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 0; // Sort by Department (column A)
            sorter.Order1 = SortOrder.Ascending;
            
            sorter.Key2 = 1; // Then by Name (column B)
            sorter.Order2 = SortOrder.Descending;
            
            sorter.Key3 = 2; // Finally by Salary (column C)
            sorter.Order3 = SortOrder.Ascending;
            
            sorter.CaseSensitive = false;

            // Определите диапазон для сортировки (заголовки + 4 строки данных)
            CellArea range = new CellArea();
            range.StartRow = 0;
            range.StartColumn = 0;
            range.EndRow = 4;
            range.EndColumn = 2;

            // Выполните сортировку
            sorter.Sort(cells, range);

            // Выведите отсортированные данные
            Console.WriteLine("Sorted Data:");
            for (int row = 0; row <= 4; row++)
            {
                Console.WriteLine($"{cells[row, 0].StringValue}, {cells[row, 1].StringValue}, {cells[row, 2].IntValue}");
            }
        }
    }
}
```

### См. также

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


