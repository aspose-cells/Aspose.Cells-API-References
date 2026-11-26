---
title: "ImportTableOptions.CheckMergedCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Указывает, следует ли проверять объединённые ячейки"
type: docs
url: /ru/net/aspose.cells/importtableoptions/checkmergedcells/
---
## ImportTableOptions.CheckMergedCells property

Указывает, проверять ли объединённые ячейки.

```csharp
public bool CheckMergedCells { get; set; }
```

### Примеры

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Customer1
    {
        public int CustomerId { get; set; }
        public string Name { get; set; }
    }

    public class ImportTableOptionsPropertyCheckMergedCellsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте объединённые ячейки для демонстрации
            worksheet.Cells.Merge(3, 3, 2, 1); // Merge D4:D5
            worksheet.Cells[3, 3].PutValue("MergedValue");

            // Создать примерные данные
            List<Customer1> customers = new List<Customer1>
            {
                new Customer1 { CustomerId = 1, Name = "Customer1" },
                new Customer1 { CustomerId = 2, Name = "Customer2" },
                new Customer1 { CustomerId = 3, Name = "Customer3" }
            };

            // Установите параметры импорта с включённым CheckMergedCells
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = false,
                InsertRows = true,
                CheckMergedCells = true
            };

            // Импортировать данные
            worksheet.Cells.ImportCustomObjects(customers, 0, 0, options);

            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Проверьте, что объединённые ячейки сохранены
            Cell mergedCell = worksheet.Cells["D4"];
            Console.WriteLine($"Merged cell value: {mergedCell.StringValue}");
            Console.WriteLine($"Is cell merged: {mergedCell.IsMerged}");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


