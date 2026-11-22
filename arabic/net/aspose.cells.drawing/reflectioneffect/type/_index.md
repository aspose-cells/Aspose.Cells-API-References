---
title: "ReflectionEffect.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReflectionEffect. تحصل وتضبط تأثير الانعكاس المحدد مسبقًا"
type: docs
url: /ar/net/aspose.cells.drawing/reflectioneffect/type/
---
## ReflectionEffect.Type property

يحصل ويضبط تأثير الانعكاس المحدد مسبقًا.

```csharp
public ReflectionEffectType Type { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // احصل على تأثير الانعكاس
            ReflectionEffect reflection = shape.Reflection;
            
            // عرض خاصية Type
            Console.WriteLine("Initial reflection type: " + reflection.Type);
            
            // تغيير نوع الانعكاس
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            Console.WriteLine("Updated reflection type: " + reflection.Type);
            
            // ضبط خصائص الانعكاس الأخرى
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // احفظ المصنف
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### انظر أيضًا

* enum [ReflectionEffectType](../../reflectioneffecttype/)
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


