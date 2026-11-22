---
title: "تعداد LineType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.LineType. يحدد نوع حد الصورة أو خط المخطط"
type: docs
url: /ar/net/aspose.cells.drawing/linetype/
---
## LineType enumeration

يحدد نوع حد [`Picture`](../picture/) أو خط [`Chart`](../../aspose.cells.charts/chart/).

```csharp
public enum LineType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DarkGray | `6` | يمثل خطًا رماديًا داكنًا. |
| Dash | `1` | يمثل خطًا متقطعًا. |
| DashDot | `3` | يمثل خطًا متقطعًا بنقطة |
| DashDotDot | `4` | يمثل خطًا متقطعًا بنقطتين. |
| Dot | `2` | يمثل خطًا منقّطًا. |
| LightGray | `8` | يمثل خطًا رماديًا فاتحًا. |
| MediumGray | `7` | يمثل خطًا رماديًا متوسطًا. |
| Solid | `0` | يمثل خطًا صلبًا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class LineTypeDemo
    {
        public static void LineTypeExample()
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

            // تعيين نوع الخط لخط المحور
            categoryAxis.AxisLine.Style = LineType.DashDot;

            // تعيين لون خط المحور
            categoryAxis.AxisLine.Color = Color.Blue;

            // الوصول إلى محور القيمة الأساسي
            Axis valueAxis = chart.ValueAxis;

            // تعيين نوع الخط لخطوط الشبكة الرئيسية
            valueAxis.MajorGridLines.Style = LineType.Dot;

            // تعيين لون خطوط الشبكة الرئيسية
            valueAxis.MajorGridLines.Color = Color.Red;

            // احفظ المصنف
            workbook.Save("LineTypeExample.xlsx");

            // أخرج النتائج
            Console.WriteLine("Chart created with custom line types for axis and gridlines.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


