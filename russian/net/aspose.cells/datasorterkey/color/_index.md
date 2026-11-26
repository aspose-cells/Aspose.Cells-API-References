---
title: "DataSorterKey.Color"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorterKey. Возвращает отсортированный цвет"
type: docs
url: /ru/net/aspose.cells/datasorterkey/color/
---
## DataSorterKey.Color property

Получает отсортированный цвет.

```csharp
public Color Color { get; }
```

### Примечания

Действует только когда [`Type`](../type/) имеет значение CellColor или FontColor.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyColorDemo
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

            // Выведите свойство цвета из ключей
            foreach (DataSorterKey k in sorter.Keys)
            {
                Console.WriteLine($"Color: {k.Color}");
            }
        }
    }
}
```

### См. также

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


