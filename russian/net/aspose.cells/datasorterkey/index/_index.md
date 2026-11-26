---
title: "DataSorterKey.Index"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorterKey. Возвращает индекс отсортированного столбца, абсолютную позицию: столбец A = 0, B = 1"
type: docs
url: /ru/net/aspose.cells/datasorterkey/index/
---
## DataSorterKey.Index property

Получает индекс отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...).

```csharp
public int Index { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIndexDemo
    {
        public static void Run()
        {
            // Создать объект рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сортировки
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Создайте сортировщик данных и добавьте ключ сортировки
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Отсортировать данные
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Продемонстрируйте использование свойства Index
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Column index being sorted: {key.Index}");
            }

            // Сохранить результат
            workbook.Save("DataSorterKeyExample.xlsx");
        }
    }
}
```

### См. также

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


