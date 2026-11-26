---
title: "DataSorter.Key1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorter. Представляет индекс первого отсортированного столбца; абсолютная позиция: столбец A — 0, B — 1"
type: docs
url: /ru/net/aspose.cells/datasorter/key1/
---
## DataSorter.Key1 property

Представляет индекс первого отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...).

```csharp
public int Key1 { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey1Demo
    {
        public static void Run()
        {
            // Создайте рабочую книгу и добавьте примерные данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);

            // Создайте сортировщик данных и установите Key1 для сортировки по столбцу Score (столбец B)
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 1; // Column index 1 (B)
            sorter.Order1 = SortOrder.Descending;

            // Определите область сортировки (строки 1‑4, все столбцы данных)
            CellArea sortArea = new CellArea();
            sortArea.StartRow = 1;
            sortArea.EndRow = 4;
            sortArea.StartColumn = 0;
            sortArea.EndColumn = cells.MaxDataColumn;

            // Выполните сортировку
            sorter.Sort(cells, sortArea);

            // Сохранить результат
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### См. также

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


