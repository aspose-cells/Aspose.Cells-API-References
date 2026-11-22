---
title: "ShadowEffect.Blur"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShadowEffect. تحصل وتعيّن تمويه الظل. النطاق من 0 إلى 100 نقطة"
type: docs
url: /ar/net/aspose.cells.drawing/shadoweffect/blur/
---
## ShadowEffect.Blur property

الحصول وتعيين تمويه الظل. النطاق من 0 إلى 100 نقطة.

```csharp
public double Blur { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف شكلًا تجريبيًا
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // احصل على تأثير الظل
            ShadowEffect shadow = shape.ShadowEffect;
            
            // ضبط خصائص الظل بما في ذلك التمويه
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Shadow effect with blur applied successfully.");
        }
    }
}
```

### انظر أيضًا

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


