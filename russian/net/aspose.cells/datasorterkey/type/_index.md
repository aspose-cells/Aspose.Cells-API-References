---
title: "DataSorterKey.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorterKey. Представляет тип сортировки"
type: docs
url: /ru/net/aspose.cells/datasorterkey/type/
---
## DataSorterKey.Type property

Представляет тип сортировки.

```csharp
public SortOnType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать объект рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Создайте сортировщик данных и добавьте ключ
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Отсортировать данные
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Продемонстрировать использование свойства Type
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Key Type: {key.Type}");
            }
        }
    }
}
```

### См. также

* enum [SortOnType](../../sortontype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


