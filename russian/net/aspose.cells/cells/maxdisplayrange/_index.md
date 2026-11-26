---
title: "Cells.MaxDisplayRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Получает максимальный диапазон, который включает данные объединённых ячеек и фигур"
type: docs
url: /ru/net/aspose.cells/cells/maxdisplayrange/
---
## Cells.MaxDisplayRange property

Получает максимальный диапазон, включающий данные, объединённые ячейки и фигуры.

```csharp
public Range MaxDisplayRange { get; }
```

### Примечания

Возвращает null, если лист пуст, начиная с Aspose.Cells 21.5.2.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDisplayRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные в ячейки, чтобы создать диапазон отображения
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Получите максимальный диапазон отображения
            Aspose.Cells.Range maxDisplayRange = worksheet.Cells.MaxDisplayRange;

            // Выведите информацию о диапазоне
            Console.WriteLine("Max Display Range:");
            Console.WriteLine($"Start Row: {maxDisplayRange.FirstRow}");
            Console.WriteLine($"Start Column: {maxDisplayRange.FirstColumn}");
            Console.WriteLine($"Total Rows: {maxDisplayRange.RowCount}");
            Console.WriteLine($"Total Columns: {maxDisplayRange.ColumnCount}");

            // Создайте новый диапазон на основе размеров максимального диапазона отображения
            Aspose.Cells.Range customRange = worksheet.Cells.CreateRange(
                maxDisplayRange.FirstRow,
                maxDisplayRange.FirstColumn,
                maxDisplayRange.RowCount,
                maxDisplayRange.ColumnCount);

            // Примените форматирование к диапазону
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;
            customRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // Сохраните книгу
            workbook.Save("MaxDisplayRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


