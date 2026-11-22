---
title: "تعداد CategoryType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Charts.CategoryType. يمثل نوع محور الفئات"
type: docs
url: /ar/net/aspose.cells.charts/categorytype/
---
## CategoryType enumeration

يمثل نوع محور الفئة.

```csharp
public enum CategoryType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| AutomaticScale | `0` | AutomaticScale |
| CategoryScale | `1` | CategoryScale |
| TimeScale | `2` | TimeScale |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CategoryTypeDemo
    {
        public static void CategoryTypeExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            // إضافة ورقة عمل جديدة إلى كائن Excel
            int sheetIndex = workbook.Worksheets.Add();
            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // إضافة قيم عينة إلى الخلايا
            worksheet.Cells["A1"].PutValue("Dates");
            worksheet.Cells["A2"].PutValue(new DateOnly(2024, 01, 01));
            worksheet.Cells["A3"].PutValue(new DateOnly(2024, 03, 01));
            worksheet.Cells["A4"].PutValue(new DateOnly(2024, 05, 01));
            worksheet.Cells["B1"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C3"].PutValue(15);
            worksheet.Cells["C4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // الوصول إلى نسخة المخطط المضاف حديثًا
            Chart chart = worksheet.Charts[chartIndex];
            // إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B3"
            chart.NSeries.Add("B2:C4", true);

            // تعيين أسماء الفئات لمحور X من النطاق "A2:A5"
            chart.NSeries[0].XValues = "A2:A4";

            // تعيين نوع محور الفئات إلى TimeScale
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;

            // تعيين مقياس الوحدة الرئيسية لمحور الفئات
            chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MajorUnit = 2;

            // تعيين مقياس الوحدة الثانوية لمحور الفئات
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // حفظ ملف Excel
            workbook.Save("CategoryTypeExample.xlsx");
            workbook.Save("CategoryTypeExample.pdf");

        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


