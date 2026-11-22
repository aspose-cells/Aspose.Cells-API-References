---
title: "ShadowEffect.Angle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShadowEffect. تحصل وتعيّن زاوية الإضاءة. النطاق من 0 إلى 359.9 درجة"
type: docs
url: /ar/net/aspose.cells.drawing/shadoweffect/angle/
---
## ShadowEffect.Angle property

يحصل ويضبط زاوية الإضاءة. النطاق من 0 إلى 359.9 درجة.

```csharp
public double Angle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyAngleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً واضبط زاوية تأثير الظل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape.ShadowEffect.Angle = 45;

            // تحقق وأخرج قيمة الزاوية
            Console.WriteLine("Shadow Effect Angle: " + shape.ShadowEffect.Angle);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


