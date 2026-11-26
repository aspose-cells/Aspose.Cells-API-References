---
title: "Cells.LastCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Возвращает последнюю ячейку в этом листе"
type: docs
url: /ru/net/aspose.cells/cells/lastcell/
---
## Cells.LastCell property

Получает последнюю ячейку в этом листе.

```csharp
public Cell LastCell { get; }
```

### Примечания

Возвращает null, если в листе нет данных.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyLastCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми данными
            worksheet.Cells["A1"].Value = "Header1";
            worksheet.Cells["B1"].Value = "Header2";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["B2"].Value = "Data2";

            // Получить адрес последней ячейки
            Cell lastCell = worksheet.Cells.LastCell;
            Console.WriteLine("Last cell address: " + lastCell.Name);

            // Создать диапазон от первой до последней ячейки
            Aspose.Cells.Range fullRange = worksheet.Cells.CreateRange(
                worksheet.Cells.FirstCell.Name, 
                lastCell.Name);
            
            // Примените форматирование к диапазону
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            fullRange.ApplyStyle(style, new StyleFlag { FontBold = true });

            // Сохраните книгу
            workbook.Save("LastCellDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


