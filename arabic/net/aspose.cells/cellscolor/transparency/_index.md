---
title: "CellsColor.Transparency"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsColor. يحصل ويعيّن الشفافية كقيمة من 0.0 غير شفاف إلى 1.0 شفاف"
type: docs
url: /ar/net/aspose.cells/cellscolor/transparency/
---
## CellsColor.Transparency property

يحصل على الشفافية ويضبطها كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

```csharp
public double Transparency { get; set; }
```

### أمثلة

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

### انظر أيضًا

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


