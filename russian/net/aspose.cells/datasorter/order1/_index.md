---
title: "DataSorter.Order1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "DataSorter property. Представляет порядок сортировки первого ключа"
type: docs
url: /ru/net/aspose.cells/datasorter/order1/
---
## DataSorter.Order1 property

Представляет порядок сортировки первого ключа.

```csharp
public SortOrder Order1 { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyOrder1Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);

            // Установить свойства сортировщика данных
            DataSorter sorter = workbook.DataSorter;
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Определить диапазон сортировки
            CellArea area = CellArea.CreateCellArea("A1", "B4");
            
            // Выполните сортировку
            sorter.Sort(worksheet.Cells, area);
            
            // Сохраните книгу
            workbook.Save("SortedOutput.xlsx");
        }
    }
}
```

### См. также

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


