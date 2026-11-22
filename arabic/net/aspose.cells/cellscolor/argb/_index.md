---
title: "CellsColor.Argb"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsColor. يحصل ويعيّن اللون من قيمة ARGB 32 بت"
type: docs
url: /ar/net/aspose.cells/cellscolor/argb/
---
## CellsColor.Argb property

يحصل على اللون ويضبطه من قيمة ARGB 32-بت.

```csharp
public int Argb { get; set; }
```

### أمثلة

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

            // إنشاء نطاق ونمط
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A5");
            Style style = workbook.CreateStyle();

            // إنشاء وتكوين CellsColor باستخدام خاصية Argb
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Argb = Color.FromArgb(128, 0, 0, 255).ToArgb(); // Semi-transparent blue

            // تطبيق اللون على النمط
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            
            // تطبيق النمط على النطاق
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // احفظ المصنف
            workbook.Save("CellsColorArgbDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


