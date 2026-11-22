---
title: "SolidFill.Color"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SolidFill. يسترجع أو يضبط اللون"
type: docs
url: /ar/net/aspose.cells.drawing/solidfill/color/
---
## SolidFill.Color property

يحصل على اللون أو يضبطه.

```csharp
public Color Color { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل مع المعلمات الصحيحة
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // تعيين خصائص الشكل باللون
            Color fillColor = Color.LightBlue;
            Color textColor = Color.DarkBlue;
            string text = "Solid Fill Demo";

            // إظهار استخدام خاصية Color
            shape.Fill.SolidFill.Color = fillColor;
            shape.LineFormat.ForeColor = fillColor;
            shape.Text = text;
            shape.Font.Color = textColor;

            // احفظ المصنف
            workbook.Save("SolidFillPropertyColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


