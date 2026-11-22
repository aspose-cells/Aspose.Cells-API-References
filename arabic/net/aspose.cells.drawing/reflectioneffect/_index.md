---
title: "الفئة ReflectionEffect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.ReflectionEffect class. هذه الفئة تحدد تأثير الانعكاس"
type: docs
url: /ar/net/aspose.cells.drawing/reflectioneffect/
---
## ReflectionEffect class

هذه الفئة تحدد تأثير الانعكاس.

```csharp
public class ReflectionEffect
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Blur](../../aspose.cells.drawing/reflectioneffect/blur/) { get; set; } | يحصل ويضبط نصف قطر الضبابية,بوحدة النقاط. |
| [Direction](../../aspose.cells.drawing/reflectioneffect/direction/) { get; set; } | يحصل ويضبط اتجاه منحدر تدرج ألفا بالنسبة إلى الشكل نفسه. |
| [Distance](../../aspose.cells.drawing/reflectioneffect/distance/) { get; set; } | يحصل ويضبط مدى إبعاد الظل,بوحدة النقاط. |
| [FadeDirection](../../aspose.cells.drawing/reflectioneffect/fadedirection/) { get; set; } | يحصل ويضبط اتجاه إزاحة الانعكاس. |
| [RotWithShape](../../aspose.cells.drawing/reflectioneffect/rotwithshape/) { get; set; } | يحصل ويضبط ما إذا كان الانعكاس يجب أن يدور مع الشكل. |
| [Size](../../aspose.cells.drawing/reflectioneffect/size/) { get; set; } | يحصل ويضبط موضع النهاية (على طول منحدر تدرج ألفا) لقيمة ألفا النهائية,بوحدة النسبة المئوية |
| [Transparency](../../aspose.cells.drawing/reflectioneffect/transparency/) { get; set; } | يحصل ويضبط درجة شفافية الانعكاس الابتدائية كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [Type](../../aspose.cells.drawing/reflectioneffect/type/) { get; set; } | يحصل ويضبط تأثير الانعكاس المحدد مسبقًا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا تجريبيًا
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // عيّن خصائص تأثير الانعكاس
            ReflectionEffect reflection = shape.Reflection;
            reflection.Size = 90;
            reflection.Blur = 30;
            reflection.Transparency = 0.5;
            reflection.Distance = 10;

            // اعرض خصائص الانعكاس
            Console.WriteLine("Reflection Size: " + reflection.Size);
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
            Console.WriteLine("Reflection Transparency: " + reflection.Transparency);
            Console.WriteLine("Reflection Distance: " + reflection.Distance);

            // احفظ المصنف
            workbook.Save("ReflectionEffectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


