---
title: "ShadowEffect.Transparency"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShadowEffect. تحصل وتعيّن درجة شفافية الظل. النطاق من 0.0 غير شفاف إلى 1.0 شفاف تمامًا"
type: docs
url: /ar/net/aspose.cells.drawing/shadoweffect/transparency/
---
## ShadowEffect.Transparency property

يحصل على ويضبط درجة شفافية الظل. النطاق من 0.0 (معتم) إلى 1.0 (شفاف).

```csharp
public double Transparency { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف شكلاً لتوضيح تأثير الظل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // احصل على تأثير الظل واضبط الخصائص بما في ذلك الشفافية
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4; // Setting transparency to 40%
            shadow.Distance = 80;
            
            // احفظ المصنف
            workbook.Save("ShadowEffectDemo.xlsx");
            
            Console.WriteLine("Workbook saved with shadow effect transparency set to 0.4");
        }
    }
}
```

### انظر أيضًا

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


