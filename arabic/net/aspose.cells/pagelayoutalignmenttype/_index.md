---
title: "تعداد PageLayoutAlignmentType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.PageLayoutAlignmentType. يعدد أنواع محاذاة تخطيط الصفحة"
type: docs
url: /ar/net/aspose.cells/pagelayoutalignmenttype/
---
## PageLayoutAlignmentType enumeration

يسرد أنواع محاذاة تخطيط الصفحة.

```csharp
public enum PageLayoutAlignmentType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Bottom | `0` | يمثل محاذاة تخطيط الصفحة السفلية. |
| Center | `1` | يمثل محاذاة تخطيط الصفحة الوسطية. |
| Left | `2` | يمثل محاذاة تخطيط الصفحة اليسرى. |
| Right | `3` | يمثل محاذاة تخطيط الصفحة اليمنى. |
| Top | `4` | يمثل محاذاة تخطيط الصفحة العليا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageLayoutAlignmentTypeDemo
    {
        public static void PageLayoutAlignmentTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);
            worksheet.Cells["A4"].PutValue(789);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // تحديد نطاق البيانات للمخطط
            chart.SetChartDataRange("A1:A4", true);

            // تحديد عنوان المخطط
            chart.Title.Text = "Sample Chart";

            // حفظ المصنف إلى ملف
            workbook.Save("PageLayoutAlignmentTypeExample.xlsx");

            // تصدير المخطط إلى ملف PDF مع محاذاة تخطيط صفحة محددة
            chart.ToPdf("ChartExample.pdf", 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


