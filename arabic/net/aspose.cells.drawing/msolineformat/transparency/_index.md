---
title: "MsoLineFormat.Transparency"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoLineFormat. تُرجع أو تُعيّن درجة الشفافية للملء المحدد كقيمة من 0.0 غير شفاف إلى 1.0 شفاف"
type: docs
url: /ar/net/aspose.cells.drawing/msolineformat/transparency/
---
## MsoLineFormat.Transparency property

إرجاع أو تعيين درجة الشفافية للملء المحدد كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

```csharp
public double Transparency { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل قوس
            ArcShape arc = worksheet.Shapes.AddArc(1, 0, 1, 0, 100, 100);

            // تعيين خصائص تنسيق الخط بما في ذلك الشفافية
            arc.LineFormat.ForeColor = System.Drawing.Color.Red;
            arc.LineFormat.Transparency = 0.5; // 50% transparent
            arc.LineFormat.Weight = 3;
            arc.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // إنشاء قوس آخر للمقارنة
            ArcShape arc2 = worksheet.Shapes.AddArc(1, 2, 1, 2, 100, 100);
            arc2.LineFormat.ForeColor = System.Drawing.Color.Red;
            arc2.LineFormat.Transparency = 0.5; // Same transparency
            arc2.LineFormat.Weight = 3;
            arc2.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // تحقق من خاصية الشفافية
            if (Math.Abs(arc.LineFormat.Transparency - arc2.LineFormat.Transparency) < 0.001)
            {
                Console.WriteLine("Transparency properties match: " + arc.LineFormat.Transparency);
            }
            else
            {
                Console.WriteLine("Transparency properties do not match");
            }

            // احفظ المصنف
            workbook.Save("MsoLineFormatTransparencyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


