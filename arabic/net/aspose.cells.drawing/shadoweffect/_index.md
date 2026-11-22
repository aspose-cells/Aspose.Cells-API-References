---
title: "فئة ShadowEffect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.ShadowEffect. تحدد هذه الفئة تأثير الظل لعنصر المخطط أو الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shadoweffect/
---
## ShadowEffect class

هذه الفئة تحدد تأثير الظل لعنصر المخطط أو الشكل.

```csharp
public class ShadowEffect
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Angle](../../aspose.cells.drawing/shadoweffect/angle/) { get; set; } | يحصل ويضبط زاوية الإضاءة. النطاق من 0 إلى 359.9 درجة. |
| [Blur](../../aspose.cells.drawing/shadoweffect/blur/) { get; set; } | الحصول وتعيين تمويه الظل. النطاق من 0 إلى 100 نقطة. |
| [Color](../../aspose.cells.drawing/shadoweffect/color/) { get; set; } | الحصول وتعيين لون الظل. |
| [Distance](../../aspose.cells.drawing/shadoweffect/distance/) { get; set; } | الحصول وتعيين مسافة الظل. النطاق من 0 إلى 200 نقطة. |
| [PresetType](../../aspose.cells.drawing/shadoweffect/presettype/) { get; set; } | يحصل على ويضبط نوع الظل المحدد مسبقًا للظل. |
| [Size](../../aspose.cells.drawing/shadoweffect/size/) { get; set; } | يحصل على ويضبط حجم الظل. النطاق من 0 إلى 2.0. غير ذي معنى في الظل الداخلي. |
| [Transparency](../../aspose.cells.drawing/shadoweffect/transparency/) { get; set; } | يحصل على ويضبط درجة شفافية الظل. النطاق من 0.0 (معتم) إلى 1.0 (شفاف). |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShadowEffectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا نموذجيًا مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // احصل على تأثير الظل للشكل
            ShadowEffect shadow = shape.ShadowEffect;

            // اضبط خصائص الظل
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // احفظ المصنف
            workbook.Save("output.xlsx");

            Console.WriteLine("Shadow effect demo completed successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


