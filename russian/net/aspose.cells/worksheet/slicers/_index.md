---
title: "Worksheet.Slicers"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получить коллекцию Slicer в листе"
type: docs
url: /ru/net/aspose.cells/worksheet/slicers/
---
## Worksheet.Slicers property

Получить коллекцию Slicer в листе

```csharp
public SlicerCollection Slicers { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetPropertySlicersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные для таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);

            // Добавить таблицу
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Добавить slicers в worksheet
            worksheet.Slicers.Add(table, table.ListColumns[0], 1, 3);
            worksheet.Slicers.Add(table, 1, "D1");
            worksheet.Slicers.Add(table, table.ListColumns[0], "G1");

            // Сохраните книгу
            workbook.Save("SlicersDemo.xlsx");
        }
    }
}
```

### См. также

* class [SlicerCollection](../../../aspose.cells.slicers/slicercollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


