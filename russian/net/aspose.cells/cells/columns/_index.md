---
title: "Cells.Columns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Возвращает коллекцию объектов Column, представляющих отдельные столбцы в этом листе"
type: docs
url: /ru/net/aspose.cells/cells/columns/
---
## Cells.Columns property

Возвращает коллекцию объектов [`Column`](../../column/), представляющих отдельные столбцы в этом листе.

```csharp
public ColumnCollection Columns { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyColumnsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите стиль для столбца 5
            Style columnStyle = workbook.CreateStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 12;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { FontName = true, FontSize = true, FontBold = true });

            // Установите ширину для столбца 5
            cells.Columns[5].Width = 20;

            // Установите данные в столбце 5, чтобы продемонстрировать стиль
            for (int row = 0; row < 10; row++)
            {
                cells[row, 5].PutValue($"Row {row + 1}");
            }

            // Сохраните книгу
            workbook.Save("ColumnsPropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [ColumnCollection](../../columncollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


