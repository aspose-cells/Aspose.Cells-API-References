---
title: "تعداد QuartileCalculationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.QuartileCalculationType تعداد. يمثل طرق حساب الربعيات"
type: docs
url: /ar/net/aspose.cells.charts/quartilecalculationtype/
---
## QuartileCalculationType enumeration

يمثل طرق حساب الأرباع.

```csharp
public enum QuartileCalculationType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Exclusive | `0` | تشمل حساب الربعيات الوسيط عند تقسيم مجموعة البيانات إلى أرباع. |
| Inclusive | `1` | تستثني حساب الربعيات الوسيط عند تقسيم مجموعة البيانات إلى أرباع. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class QuartileCalculationTypeDemo
    {
        public static void QuartileCalculationTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات النموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة سلسلة إلى المخطط
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // الوصول إلى خصائص تخطيط السلسلة
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // تعيين نوع حساب الربعيات
            layoutProperties.QuartileCalculation = QuartileCalculationType.Exclusive;

            // احفظ المصنف
            workbook.Save("QuartileCalculationTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


