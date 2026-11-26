---
title: "CellsColor.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsColor. Получает и задает прозрачность значением от 0.0 (непрозрачный) до 1.0 (полностью прозрачный)"
type: docs
url: /ru/net/aspose.cells/cellscolor/transparency/
---
## CellsColor.Transparency property

Получает и задает прозрачность в диапазоне от 0,0 (непрозрачный) до 1,0 (прозрачный).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyTransparencyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Color = Color.FromArgb(128, 255, 0, 0); // Semi-transparent red
            cellsColor.Transparency = 0.5; // Set transparency to 50%

            Style style = workbook.CreateStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;

            worksheet.Cells["A1"].PutValue("50% transparent red background");
            worksheet.Cells["A1"].SetStyle(style);

            workbook.Save("TransparencyDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


