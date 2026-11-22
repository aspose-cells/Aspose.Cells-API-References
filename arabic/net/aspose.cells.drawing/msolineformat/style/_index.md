---
title: "MsoLineFormat.Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoLineFormat. تُرجع كائن Style يمثل نمط النطاق المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/msolineformat/style/
---
## MsoLineFormat.Style property

يرجع كائن Style يمثل نمط النطاق المحدد.

```csharp
public MsoLineStyle Style { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل خط
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 150, 10, 10);

            // احصل على تنسيق الخط
            MsoLineFormat lineFormat = line.LineFormat;

            // تعيين خصائص نمط الخط
            lineFormat.Style = MsoLineStyle.ThickBetweenThin;
            lineFormat.ForeColor = System.Drawing.Color.Red;
            lineFormat.BackColor = System.Drawing.Color.White;
            lineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 3.0;

            // إنشاء خط آخر للمقارنة
            Aspose.Cells.Drawing.LineShape line2 = worksheet.Shapes.AddLine(5, 25, 100, 150, 10, 10);
            MsoLineFormat lineFormat2 = line2.LineFormat;

            // نسخ النمط من الخط الأول إلى الخط الثاني
            lineFormat2.Style = lineFormat.Style;
            lineFormat2.ForeColor = lineFormat.ForeColor;
            lineFormat2.BackColor = lineFormat.BackColor;
            lineFormat2.DashStyle = lineFormat.DashStyle;
            lineFormat2.Transparency = lineFormat.Transparency;
            lineFormat2.Weight = lineFormat.Weight;

            // احفظ المصنف
            workbook.Save("MsoLineFormatStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


