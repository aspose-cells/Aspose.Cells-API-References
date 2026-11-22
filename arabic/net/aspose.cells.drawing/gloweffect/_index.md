---
title: "الفئة GlowEffect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.GlowEffect. تحدد هذه الفئة تأثير توهج يتم فيه إضافة حد ملون مشوش خارج حواف الكائن"
type: docs
url: /ar/net/aspose.cells.drawing/gloweffect/
---
## GlowEffect class

تحدد هذه الفئة تأثير التوهج، حيث يُضاف حد ملون ضبابي خارج حواف الكائن.

```csharp
public class GlowEffect
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Color](../../aspose.cells.drawing/gloweffect/color/) { get; set; } | الحصول على لون تأثير التوهج. |
| [Radius](../../aspose.cells.drawing/gloweffect/radius/) { get; set; } | (**Obsolete.**) الحصول على وتعيين نصف قطر التوهج، بوحدة النقاط. |
| [Size](../../aspose.cells.drawing/gloweffect/size/) { get; set; } | الحصول على وتعيين نصف قطر التوهج، بوحدة النقاط. |
| [Transparency](../../aspose.cells.drawing/gloweffect/transparency/) { get; set; } | الحصول على وتعيين درجة شفافية تأثير التوهج. النطاق من 0.0 (معتم) إلى 1.0 (شفاف). |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GlowEffectDemo
    {
        public static void GlowEffectExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً قوسيًا إلى ورقة العمل
            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // تعيين موضع القوس
            arcShape.Placement = PlacementType.FreeFloating;

            // تعيين تنسيق التعبئة
            arcShape.Fill.FillType = FillType.Solid;
            arcShape.Fill.SolidFill.Color = Color.Blue;

            // تعيين نمط الخط
            arcShape.Line.CompoundType = MsoLineStyle.Single;
            arcShape.Line.Weight = 2;
            arcShape.Line.FillType = FillType.Solid;
            arcShape.Line.SolidFill.Color = Color.Red;
            arcShape.Line.DashStyle = MsoLineDashStyle.Solid;

            // إنشاء مثيل GlowEffect وتعيين خصائصه
            GlowEffect glowEffect = arcShape.Glow;
            glowEffect.Color = workbook.CreateCellsColor();
            glowEffect.Color.Color = Color.Yellow;
            glowEffect.Radius = 10.0;
            glowEffect.Transparency = 0.5;

            // احفظ المصنف
            workbook.Save("GlowEffectExample.xlsx");
            workbook.Save("GlowEffectExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


