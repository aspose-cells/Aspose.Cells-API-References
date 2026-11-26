---
title: "DataSorter.Key3"
second_title: "Справочник API Aspose.Cells для .NET"
description: "DataSorter property. Представляет индекс третьего отсортированного столбца, абсолютная позиция: столбец A = 0, B = 1"
type: docs
url: /ru/net/aspose.cells/datasorter/key3/
---
## DataSorter.Key3 property

Представляет индекс третьего отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...).

```csharp
public int Key3 { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey3Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["C1"].PutValue("Grade");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["C2"].PutValue("B");
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["C3"].PutValue("A");
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);
            cells["C4"].PutValue("C");
            cells["A5"].PutValue("Eve");
            cells["B5"].PutValue(92);
            cells["C5"].PutValue("A");

            // Создать сортировщик данных
            DataSorter sorter = workbook.DataSorter;
            
            // Сортировать по Score (по убыванию), затем по Name (по возрастанию), затем по Grade (по убыванию)
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Column B (Score)
            
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 0; // Column A (Name)
            
            sorter.Order3 = SortOrder.Descending;
            sorter.Key3 = 2; // Column C (Grade)
            
            // Отсортировать диапазон данных
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 5, 2));

            // Сохраните книгу
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### См. также

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


