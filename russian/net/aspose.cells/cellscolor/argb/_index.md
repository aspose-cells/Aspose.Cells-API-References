---
title: "CellsColor.Argb"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsColor. Получает и задает цвет из 32‑битного значения ARGB"
type: docs
url: /ru/net/aspose.cells/cellscolor/argb/
---
## CellsColor.Argb property

Получает и задает цвет из 32‑битного значения ARGB.

```csharp
public int Argb { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyArgbDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать диапазон и стиль
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A5");
            Style style = workbook.CreateStyle();

            // Создать и настроить CellsColor, используя свойство Argb
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Argb = Color.FromArgb(128, 0, 0, 255).ToArgb(); // Semi-transparent blue

            // Применить цвет к стилю
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            
            // Применить стиль к диапазону
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Сохраните книгу
            workbook.Save("CellsColorArgbDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


