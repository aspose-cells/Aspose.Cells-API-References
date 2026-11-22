---
title: "التعداد MsoLineDashStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.MsoLineDashStyle. يمثل نمط خطوط الرسم المتقطعة"
type: docs
url: /ar/net/aspose.cells.drawing/msolinedashstyle/
---
## MsoLineDashStyle enumeration

يمثل نمط الخطوط المتقطعة.

```csharp
public enum MsoLineDashStyle
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Dash | `0` | يمثل خطًا متقطعًا. |
| DashDot | `1` | يمثل خطًا متقطّعًا-نقطة. |
| DashDotDot | `2` | يمثل خطًا متقطعًا بنقطتين. |
| DashLongDash | `3` | يمثل خطًا متقطّعًا طويلًا-قصيرًا. |
| DashLongDashDot | `4` | يمثل خطًا متقطّعًا طويلًا-قصيرًا-نقطة. |
| RoundDot | `5` | يمثل خطًا بنقطة دائرية. |
| Solid | `6` | يمثل خطًا صلبًا. |
| SquareDot | `7` | يمثل خطًا بنقطة مربعة. |
| Custom | `8` | نمط متقطّع مخصص. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineDashStyleDemo
    {
        public static void MsoLineDashStyleExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            // الوصول إلى محور الفئة الأساسي
            Axis categoryAxis = chart.CategoryAxis;

            // تعيين نمط المتقطّع لخطوط الشبكة الرئيسية
            categoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;

            // تعيين نمط المتقطّع لخطوط الشبكة الفرعية
            categoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // احفظ المصنف
            workbook.Save("MsoLineDashStyleExample.xlsx");

            // أخرج النتائج
            Console.WriteLine("Chart with custom dash styles for gridlines created successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


