---
title: "CellsColor.Color"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsColor. Получает и задает цвет RGB"
type: docs
url: /ru/net/aspose.cells/cellscolor/color/
---
## CellsColor.Color property

Получает и задает цвет RGB.

```csharp
public Color Color { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать диапазон и установить цветные границы
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical, CellBorderType.Thin, color);

            // Проверьте настройки границ в ячейке
            Cell cell = worksheet.Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            // Сохраните книгу
            workbook.Save("CellsColorPropertyColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


