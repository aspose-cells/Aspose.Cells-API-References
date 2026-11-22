---
title: "ShadowEffect.Size"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShadowEffect. تحصل وتعيّن حجم الظل. النطاق من 0 إلى 2.0. غير ذات معنى في الظل الداخلي"
type: docs
url: /ar/net/aspose.cells.drawing/shadoweffect/size/
---
## ShadowEffect.Size property

يحصل على ويضبط حجم الظل. النطاق من 0 إلى 2.0. غير ذي معنى في الظل الداخلي.

```csharp
public double Size { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertySizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook book = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإضافة شكل
            Worksheet sheet = book.Worksheets[0];
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // احصل على تأثير الظل واضبط الخصائص بما في ذلك الحجم
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3; // Demonstrating Size property usage
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // احفظ المصنف
            book.Save("ShadowEffectExample.xlsx");
            
            Console.WriteLine("Shadow effect with Size property set to 1.3 has been applied.");
        }
    }
}
```

### انظر أيضًا

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


