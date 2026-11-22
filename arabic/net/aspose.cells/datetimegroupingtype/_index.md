---
title: "تعداد DateTimeGroupingType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.DateTimeGroupingType. يحدد كيفية تجميع قيم التاريخ والوقت"
type: docs
url: /ar/net/aspose.cells/datetimegroupingtype/
---
## DateTimeGroupingType enumeration

يحدد كيفية تجميع قيم التاريخ والوقت.

```csharp
public enum DateTimeGroupingType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Day | `0` | تجميع حسب اليوم. |
| Hour | `1` | تجميع حسب الساعة. |
| Minute | `2` | تجميع حسب الدقيقة. |
| Month | `3` | تجميع حسب الشهر. |
| Second | `4` | تجميع حسب الثانية. |
| Year | `5` | تجميع حسب السنة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupingTypeDemo
    {
        public static void DateTimeGroupingTypeExample()
        {
            // إنشاء مصنف والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1, 10, 0, 0));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1, 11, 0, 0));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2, 10, 0, 0));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 2, 11, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 2, 1, 10, 0, 0));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 2, 1, 11, 0, 0));

            // إنشاء مرشح تلقائي وتحديد النطاق
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:A6";

            // إضافة مرشحات تاريخ بأنواع DateTimeGroupingType مختلفة
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Month, 2023, 1, 1, 0, 0, 0);
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Hour, 2023, 1, 1, 10, 0, 0);
            
            // حفظ المصنف
            workbook.Save("DateTimeGroupingTypeExample.xlsx");
            workbook.Save("DateTimeGroupingTypeExample.pdf");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


