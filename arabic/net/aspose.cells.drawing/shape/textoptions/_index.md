---
title: "Shape.TextOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل خيارات النص للشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/textoptions/
---
## Shape.TextOptions property

يمثل خيارات النص للشكل.

```csharp
public TextOptions TextOptions { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // تعيين النص للشكل
            shape.Text = "Sample Text";

            // الوصول إلى TextOptions وتعديلها
            TextOptions opt = shape.TextOptions;
            opt.Color = Color.Blue;
            opt.Size = 8;

            // احفظ المصنف
            workbook.Save("ShapeTextOptionsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


