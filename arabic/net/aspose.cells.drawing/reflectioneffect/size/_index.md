---
title: "ReflectionEffect.Size"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReflectionEffect. تحصل وتضبط موضع النهاية على طول منحدر تدرج ألفا لقيمة ألفا النهائية بوحدة النسبة المئوية"
type: docs
url: /ar/net/aspose.cells.drawing/reflectioneffect/size/
---
## ReflectionEffect.Size property

يحصل ويضبط موضع النهاية (على طول منحدر تدرج ألفا) لقيمة ألفا النهائية,بوحدة النسبة المئوية

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
    public class ReflectionEffectPropertySizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // اضبط خصائص الانعكاس بما في ذلك الحجم
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4;

            // احفظ المصنف
            workbook.Save("output.xlsx");

            // تحقق من خصائص الانعكاس المحفوظة
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Reflection Size: " + loadedReflection.Size);
        }
    }
}
```

### انظر أيضًا

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


