---
title: "DataSorter.Keys"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorter. Возвращает список ключей сортировщика данных"
type: docs
url: /ru/net/aspose.cells/datasorter/keys/
---
## DataSorter.Keys property

Получает список ключей сортировщика данных.

```csharp
public DataSorterKeyCollection Keys { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKeysDemo
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

            // Инициализировать сортировщик данных
            DataSorter sorter = workbook.DataSorter;
            
            // Добавить ключ сортировки для столбца A (индекс 0)
            sorter.AddKey(0, SortOrder.Ascending);

            // Отсортировать данные
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Продемонстрировать использование свойства Keys
            DataSorterKeyCollection keys = sorter.Keys;
            Console.WriteLine("Sort Keys Information:");
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Column Index: {key.Index}, Sort Order: {key.Order}");
            }

            // Сохраните книгу
            workbook.Save("DataSorterKeysDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataSorterKeyCollection](../../datasorterkeycollection/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


