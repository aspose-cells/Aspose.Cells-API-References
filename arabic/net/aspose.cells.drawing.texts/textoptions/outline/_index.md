---
title: "TextOptions.Outline"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextOptions. تمثل تنسيق المخطط للنص"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textoptions/outline/
---
## TextOptions.Outline property

يمثل تنسيق المخطط للنص.

```csharp
public LineFormat Outline { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyOutlineDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً بنص
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            shape.Text = "Sample Text";

            // الوصول إلى خيارات النص
            TextOptions textOptions = shape.TextOptions;

            // تكوين خصائص المخطط
            LineFormat outline = textOptions.Outline;
            outline.Weight = 2.48; // Set outline weight
            outline.DashStyle = MsoLineDashStyle.Solid; // Set line style
            outline.CompoundType = MsoLineStyle.Single; // Set compound type

            // احفظ المصنف
            workbook.Save("TextOutlineDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LineFormat](../../../aspose.cells.drawing/lineformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


