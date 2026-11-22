---
title: "MsoLineFormat.DashStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoLineFormat. تحصل أو تعيّن نمط الخط المتقطع للخط المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/msolineformat/dashstyle/
---
## MsoLineFormat.DashStyle property

يحصل على أو يضبط نمط الشرط للخط المحدد.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyDashStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة شكل لتوضيح DashStyle
            Shape shape = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // حدد خصائص الخط
            shape.LineFormat.Style = MsoLineStyle.Single;
            shape.LineFormat.Weight = 3;
            shape.LineFormat.ForeColor = Color.Blue;

            // توضيح أنماط خط متقطعة مختلفة
            shape.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            shape.Text = "Solid Line";

            // إضافة شكل آخر بنمط خط متقطع مختلف
            Shape shape2 = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 3, 0, 200, 100);
            shape2.LineFormat.Style = MsoLineStyle.Single;
            shape2.LineFormat.Weight = 3;
            shape2.LineFormat.ForeColor = Color.Red;
            shape2.LineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            shape2.Text = "DashDotDot Line";

            // احفظ المصنف
            workbook.Save("LineDashStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


