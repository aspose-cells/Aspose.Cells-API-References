---
title: "تعداد ChartLineFormattingType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.ChartLineFormattingType enum. يمثل نوع تنسيق الخط لخط المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartlineformattingtype/
---
## ChartLineFormattingType enumeration

يمثل نوع تنسيق الخط لخط المخطط.

```csharp
public enum ChartLineFormattingType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Automatic | `0` | يمثل نوع التنسيق التلقائي. |
| Solid | `1` | يمثل نوع التنسيق الصلب. |
| None | `2` | يمثل نوع التنسيق لا شيء. |
| Gradient | `3` | تدرج |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartLineFormattingTypeDemo
    {
        public static void ChartLineFormattingTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة إلى المخطط
            chart.NSeries.Add("A1:B3", true);
            
            // ضبط بيانات الفئة
            chart.NSeries.CategoryData = "A1:A3";
            
            // ضبط أنواع تنسيق خطوط مختلفة للسلسلة
            chart.NSeries[0].SeriesLines.FormattingType = ChartLineFormattingType.Solid;
            chart.NSeries[0].SeriesLines.Color = Color.Red;
            
            // إضافة سلسلة أخرى بتنسيق مختلف
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
            chart.NSeries[1].SeriesLines.Color = Color.Blue;
            
            // احفظ المصنف
            workbook.Save("ChartLineFormattingTypeExample.xlsx");
            workbook.Save("ChartLineFormattingTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


