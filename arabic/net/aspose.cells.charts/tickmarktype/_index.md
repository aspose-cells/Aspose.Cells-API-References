---
title: "التعداد TickMarkType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Charts.TickMarkType. يمثل نوع علامة الفاصل للمحور المحدد"
type: docs
url: /ar/net/aspose.cells.charts/tickmarktype/
---
## TickMarkType enumeration

يمثل نوع علامة التحديد للمحور المحدد.

```csharp
public enum TickMarkType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Cross | `0` | نوع علامة الفاصل هو Cross. |
| Inside | `1` | نوع علامة الفاصل هو Inside. |
| None | `2` | نوع علامة الفاصل هو None. |
| Outside | `3` | نوع علامة الفاصل هو Outside |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickMarkTypeDemo
    {
        public static void TickMarkTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // أضف NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية \"A1\" إلى \"B3\"
            chart.NSeries.Add("A1:B3", true);

            // الوصول إلى محور القيمة للمخطط
            Axis valueAxis = chart.ValueAxis;

            // تعيين نوع علامة الفاصل الرئيسية إلى Cross
            valueAxis.MajorTickMark = TickMarkType.Cross;

            // تعيين نوع علامة الفاصل الثانوية إلى Inside
            valueAxis.MinorTickMark = TickMarkType.Inside;

            // حدد القيمة القصوى لمحور القيم
            valueAxis.MaxValue = 200;

            // حدد القيمة الدنيا لمحور القيم
            valueAxis.MinValue = 0;

            // حدد الوحدة الرئيسية
            valueAxis.MajorUnit = 25;

            // احفظ المصنف
            workbook.Save("TickMarkTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


