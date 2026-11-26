---
title: "DataSorter.HasHeaders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorter. Указывает, содержит ли диапазон заголовки"
type: docs
url: /ru/net/aspose.cells/datasorter/hasheaders/
---
## DataSorter.HasHeaders property

Представляет, имеет ли диапазон заголовки.

```csharp
public bool HasHeaders { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyHasHeadersDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить заголовки и примерные данные
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["B4"].PutValue(12);

            // Создать сортировщик данных и установить HasHeaders в true
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true; // This tells the sorter the first row contains headers
            
            // Отсортировать по первому столбцу (Fruits) в порядке возрастания
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Отсортировать диапазон данных (включая заголовки)
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "B4"));

            // Сохранить отсортированную рабочую книгу
            workbook.Save("SortedWithHeaders.xlsx");
        }
    }
}
```

### См. также

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


