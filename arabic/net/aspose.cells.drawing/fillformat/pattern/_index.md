---
title: "FillFormat.Pattern"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FillFormat. تمثل نمط عرض المناطق"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/pattern/
---
## FillFormat.Pattern property

يمثل نمط عرض المنطقة.

```csharp
public FillPattern Pattern { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPatternDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue(50);
            sheet.Cells["A2"].PutValue(100);
            sheet.Cells["A3"].PutValue(150);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("A1:A3", true);

            // الوصول إلى السلسلة الأولى والنقطة الأولى فيها
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // تعيين نمط التعبئة لمنطقة النقطة
            point.Area.FillFormat.Pattern = FillPattern.DottedGrid;
            
            // احفظ المصنف
            workbook.Save("FillFormatPatternDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FillPattern](../../fillpattern/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


