---
title: "تعداد ReflectionEffectType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.ReflectionEffectType. يمثل نوع تأثير الانعكاس"
type: docs
url: /ar/net/aspose.cells.drawing/reflectioneffecttype/
---
## ReflectionEffectType enumeration

يمثل نوع تأثير الانعكاس.

```csharp
public enum ReflectionEffectType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | بدون تأثير انعكاس. |
| Custom | `1` | تأثير انعكاس مخصص. |
| TightReflectionTouching | `2` | انعكاس ضيق، ملامس. |
| HalfReflectionTouching | `3` | انعكاس نصف، ملامس. |
| FullReflectionTouching | `4` | انعكاس كامل، ملامس. |
| TightReflection4PtOffset | `5` | انعكاس ضيق، إزاحة 4 نقاط. |
| HalfReflection4PtOffset | `6` | انعكاس نصف، إزاحة 4 نقاط. |
| FullReflection4PtOffset | `7` | انعكاس كامل، إزاحة 4 نقاط. |
| TightReflection8PtOffset | `8` | انعكاس ضيق، إزاحة 8 نقاط. |
| HalfReflection8PtOffset | `9` | انعكاس نصف، إزاحة 8 نقاط. |
| FullReflection8PtOffset | `10` | انعكاس كامل، إزاحة 8 نقاط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل مستطيل
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // الحصول على تأثير الانعكاس
            ReflectionEffect reflection = rectangle.Reflection;
            
            // تعيين خصائص الانعكاس
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // احفظ المصنف
            workbook.Save("DrawingClassReflectionEffectTypeDemo.xlsx");
            
            Console.WriteLine("Reflection effect demo completed successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


