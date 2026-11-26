---
title: "Range.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Получает объект Cell в этом диапазоне"
type: docs
url: /ru/net/aspose.cells/range/item/
---
## Range indexer

Получает объект [`Cell`](../../cell/) в этом диапазоне.

```csharp
public Cell this[int rowOffset, int columnOffset] { get; }
```

| Параметр | Описание |
| --- | --- |
| rowOffset | Смещение строки в этом диапазоне, начиная с нуля. |
| columnOffset | Смещение столбца в этом диапазоне, начиная с нуля. |

### Возвращаемое значение

[`Cell`](../../cell/) object.

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangePropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные
            DataTable dt = new DataTable();
            dt.Columns.Add("Id", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Rows.Add(1001, "Item 1");
            dt.Rows.Add(1002, "Item 2");

            // Создайте диапазон и продемонстрируйте свойство Item
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B3");
            
            // Установите заголовки, используя свойство Item
            range[0, 0].PutValue("Id");
            range[0, 1].PutValue("Name");

            // Заполните данные, используя свойство Item
            for (int i = 0; i < dt.Rows.Count; i++)
            {
                range[i + 1, 0].PutValue(dt.Rows[i]["Id"]);
                range[i + 1, 1].PutValue(dt.Rows[i]["Name"]);
            }

            // Отформатируйте строку заголовка, используя свойство Item
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.FromArgb(0, 176, 80);
            range[0, 0].SetStyle(style);
            range[0, 1].SetStyle(style);

            // Сохраните книгу
            workbook.Save("RangePropertyItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


