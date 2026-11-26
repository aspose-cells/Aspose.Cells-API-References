---
title: "Класс DataSorterKey"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DataSorterKey. Представляет ключ сортировщика данных"
type: docs
url: /ru/net/aspose.cells/datasorterkey/
---
## DataSorterKey class

Представляет ключ сортировщика данных.

```csharp
public class DataSorterKey
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Color](../../aspose.cells/datasorterkey/color/) { get; } | Получает отсортированный цвет. |
| [IconId](../../aspose.cells/datasorterkey/iconid/) { get; } | Представляет идентификатор типа набора значков. |
| [IconSetType](../../aspose.cells/datasorterkey/iconsettype/) { get; } | Представляет тип набора значков. |
| [Index](../../aspose.cells/datasorterkey/index/) { get; } | Получает индекс отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...). |
| [Order](../../aspose.cells/datasorterkey/order/) { get; } | Указывает порядок сортировки. |
| [Type](../../aspose.cells/datasorterkey/type/) { get; } | Представляет тип сортировки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataSorterKeyDemo
    {
        public static void DataSorterKeyExample()
        {
            // Создайте объект рабочей книги и загрузите файл шаблона
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных для сортировки
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Создайте экземпляр объекта сортировщика данных
            DataSorter sorter = workbook.DataSorter;

            // Добавьте ключ для первого столбца (A) для сортировки по возрастанию
            sorter.AddKey(0, SortOrder.Ascending);

            // Создайте область ячеек (диапазон) для сортировки
            CellArea ca = CellArea.CreateCellArea("A1", "A5");

            // Выполните сортировку
            sorter.Sort(worksheet.Cells, ca);

            // Сохраните выходной файл
            workbook.Save("DataSorterKeyExample.xlsx");
            workbook.Save("DataSorterKeyExample.pdf");

            // Получите доступ к DataSorterKeyCollection
            DataSorterKeyCollection keys = sorter.Keys;

            // Итерируйте по ключам и выведите их свойства
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Order: {key.Order}");
                Console.WriteLine($"Index: {key.Index}");
                Console.WriteLine($"Type: {key.Type}");
                Console.WriteLine($"IconSetType: {key.IconSetType}");
                Console.WriteLine($"IconId: {key.IconId}");
                Console.WriteLine($"Color: {key.Color}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


