---
title: "التعداد LineJoinType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.LineJoinType. يمثل أنماط الوصل لخط."
type: docs
url: /ar/net/aspose.cells.drawing/linejointype/
---
## LineJoinType enumeration

يمثل أنماط الوصل للخط.

```csharp
public enum LineJoinType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Round | `0` | وصلة مستديرة |
| Bevel | `1` | وصلة مشطوفة |
| Miter | `2` | وصلة مِتر |
| None | `3` | بدون وصلة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LineJoinTypeDemo
    {
        public static void LineJoinTypeExample()
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

            // الوصول إلى محور القيمة الأساسي
            Axis valueAxis = chart.ValueAxis;

            // الوصول إلى تنسيق الخط للخطوط الشبكية الرئيسية
            Line majorGridLines = valueAxis.MajorGridLines;

            // تعيين نوع الوصلة للخط
            majorGridLines.JoinType = LineJoinType.Round;

            // إخراج نوع الوصلة
            Console.WriteLine("Line Join Type: " + majorGridLines.JoinType);

            // احفظ المصنف
            workbook.Save("LineJoinTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


