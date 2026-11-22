---
title: "ReflectionEffect.FadeDirection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReflectionEffect. تحصل وتضبط الاتجاه لإزاحة الانعكاس"
type: docs
url: /ar/net/aspose.cells.drawing/reflectioneffect/fadedirection/
---
## ReflectionEffect.FadeDirection property

يحصل ويضبط اتجاه إزاحة الانعكاس.

```csharp
public double FadeDirection { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyFadeDirectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل لتطبيق تأثير الانعكاس
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // الحصول على تأثير الانعكاس للشكل
            ReflectionEffect reflection = shape.Reflection;

            // عرض قيمة FadeDirection الحالية
            Console.WriteLine("Current FadeDirection value: " + reflection.FadeDirection);

            // تعيين قيمة FadeDirection جديدة (90 درجة)
            reflection.FadeDirection = 90;
            Console.WriteLine("New FadeDirection value: " + reflection.FadeDirection);

            // تكوين خصائص الانعكاس الأخرى لتحسين الرؤية
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            reflection.Distance = 10;

            // حفظ المصنف لرؤية التأثير
            workbook.Save("ReflectionEffectFadeDirectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


