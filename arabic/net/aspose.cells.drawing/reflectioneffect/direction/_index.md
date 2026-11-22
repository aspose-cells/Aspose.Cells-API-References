---
title: "ReflectionEffect.Direction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReflectionEffect. تحصل وتضبط اتجاه منحدر تدرج ألفا بالنسبة إلى الشكل نفسه"
type: docs
url: /ar/net/aspose.cells.drawing/reflectioneffect/direction/
---
## ReflectionEffect.Direction property

يحصل ويضبط اتجاه منحدر تدرج ألفا بالنسبة إلى الشكل نفسه.

```csharp
public double Direction { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyDirectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل لتطبيق تأثير الانعكاس
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // الحصول على تأثير الانعكاس للشكل
            ReflectionEffect reflection = shape.Reflection;
            
            // اعرض قيمة الاتجاه الحالية
            Console.WriteLine("Current Direction value: " + reflection.Direction);
            
            // تعيين قيمة Direction جديدة (90 درجة)
            reflection.Direction = 90;
            Console.WriteLine("New Direction value: " + reflection.Direction);
            
            // تكوين خصائص الانعكاس الأخرى لتحسين الرؤية
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            
            // حفظ المصنف لرؤية تأثير الانعكاس
            workbook.Save("ReflectionEffectDirectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


