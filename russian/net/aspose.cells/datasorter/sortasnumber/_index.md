---
title: "DataSorter.SortAsNumber"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorter. Указывает, следует ли сортировать всё, что выглядит как число"
type: docs
url: /ru/net/aspose.cells/datasorter/sortasnumber/
---
## DataSorter.SortAsNumber property

Указывает, сортировать ли всё, что выглядит как число.

```csharp
public bool SortAsNumber { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortAsNumberDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные со смешанными числами и числовыми строками
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Создайте область ячеек для сортировки
            CellArea ca = CellArea.CreateCellArea("A1", "A4");

            // Создать сортировщик данных
            DataSorter sorter = workbook.DataSorter;
            int idx = CellsHelper.ColumnNameToIndex("A");

            // Добавьте ключ сортировки (столбец A)
            sorter.AddKey(idx, SortOrder.Ascending);

            // Сортировать как числа (true) или как строки (false)
            sorter.SortAsNumber = true;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("Sorted as numbers:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Сбросьте данные для второй сортировки
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Сортировать как строки
            sorter.SortAsNumber = false;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("\nSorted as strings:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### См. также

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


