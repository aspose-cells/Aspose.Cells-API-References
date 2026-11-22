---
title: "ShadowEffect.Distance"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShadowEffect. تحصل وتعيّن مسافة الظل. النطاق من 0 إلى 200 نقطة"
type: docs
url: /ar/net/aspose.cells.drawing/shadoweffect/distance/
---
## ShadowEffect.Distance property

الحصول وتعيين مسافة الظل. النطاق من 0 إلى 200 نقطة.

```csharp
public double Distance { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);
            
            // تكوين تأثير الظل
            ShadowEffect shadow = rectangle.ShadowEffect;
            shadow.PresetType = PresetShadowType.OffsetDiagonalTopRight;
            
            // إنشاء كائن CellsColor وتعيين قيم ARGB
            CellsColor color = workbook.CreateCellsColor();
            color.Argb = (128 << 24) | (255 << 16) | (0 << 8) | 0; // Semi-transparent red
            shadow.Color = color;
            
            shadow.Transparency = 0.3;
            shadow.Blur = 15;
            shadow.Angle = 45;
            shadow.Distance = 20; // Set distance to 20 points

            // عرض مسافة الظل
            Console.WriteLine("Shadow Distance: " + shadow.Distance + " points");

            // حفظ دفتر العمل مع تأثير الظل
            workbook.Save("ShadowEffectPropertyDistanceDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


