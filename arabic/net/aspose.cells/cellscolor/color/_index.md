---
title: "CellsColor.Color"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsColor. يحصل ويعيّن لون RGB"
type: docs
url: /ar/net/aspose.cells/cellscolor/color/
---
## CellsColor.Color property

يحصل على اللون RGB ويضبطه.

```csharp
public Color Color { get; set; }
```

### أمثلة

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

            // إنشاء نطاق وتعيين حدود ملونة
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical, CellBorderType.Thin, color);

            // تحقق من إعدادات الحدود في خلية
            Cell cell = worksheet.Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            // احفظ المصنف
            workbook.Save("CellsColorPropertyColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


