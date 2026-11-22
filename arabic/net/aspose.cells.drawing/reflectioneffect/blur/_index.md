---
title: "ReflectionEffect.Blur"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReflectionEffect. تحصل وتضبط نصف قطر الضبابية بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/reflectioneffect/blur/
---
## ReflectionEffect.Blur property

يحصل ويضبط نصف قطر الضبابية,بوحدة النقاط.

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
    public class ReflectionEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل مستطيل
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // الوصول إلى تأثير الانعكاس
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            
            // ضبط نوع الانعكاس والخصائص
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Blur = 0.5; // Demonstrate Blur property
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Distance = 0;
            
            // احفظ المصنف
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // عرض قيمة الضبابية
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
        }
    }
}
```

### انظر أيضًا

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


