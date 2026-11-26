---
title: "DataSorterKeyCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorterKeyCollection. Получает и задает DataSorterKey по индексу"
type: docs
url: /ru/net/aspose.cells/datasorterkeycollection/item/
---
## DataSorterKeyCollection indexer

Получает и задает [`DataSorterKey`](../../datasorterkey/) по индексу.

```csharp
public DataSorterKey this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class DataSorterKeyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["B4"].PutValue(78);

            // Создайте объект списка (таблица)
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Добавьте ключ сортировки (сортировать по столбцу Score по убыванию)
            table.AutoFilter.Sorter.AddKey(1, SortOrder.Descending);
            table.AutoFilter.Sorter.Sort();

            // Продемонстрировать использование свойства Item
            DataSorterKey key = table.AutoFilter.Sorter.Keys[0];
            Console.WriteLine("Sort Key Index: {0}, Order: {1}", key.Index, key.Order);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [DataSorterKey](../../datasorterkey/)
* class [DataSorterKeyCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


