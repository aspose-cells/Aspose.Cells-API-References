---
title: "تعداد TickLabelAlignmentType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Charts.TickLabelAlignmentType. يمثل نوع محاذاة النص لتسميات العلامات على المحور"
type: docs
url: /ar/net/aspose.cells.charts/ticklabelalignmenttype/
---
## TickLabelAlignmentType enumeration

يمثل نوع محاذاة النص لتسميات العلامات على المحور

```csharp
public enum TickLabelAlignmentType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Center | `0` | يحدد أن النص مُوسَّط. |
| Left | `1` | يحدد أن النص مُحاذى إلى اليسار. |
| Right | `2` | يحدد أن النص محاذى إلى اليمين.. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelAlignmentTypeDemo
    {
        public static void TickLabelAlignmentTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
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

            // إضافة سلسلة إلى المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى تسميات العلامات على محور الفئة
            TickLabels tickLabels = chart.CategoryAxis.TickLabels;

            // تعيين نوع المحاذاة لتسميات العلامات
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // احفظ المصنف
            workbook.Save("TickLabelAlignmentTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


