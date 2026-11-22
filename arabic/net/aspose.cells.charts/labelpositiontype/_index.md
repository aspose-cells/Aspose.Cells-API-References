---
title: "تعداد LabelPositionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Charts.LabelPositionType. يمثل نوع موضع تسمية البيانات"
type: docs
url: /ar/net/aspose.cells.charts/labelpositiontype/
---
## LabelPositionType enumeration

يمثل نوع موضع تسمية البيانات.

```csharp
public enum LabelPositionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Center | `0` | ينطبق فقط على المخططات الشريطية ومخططات الفطيرة ثنائية/ثلاثية الأبعاد |
| InsideBase | `1` | ينطبق فقط على المخططات الشريطية ومخططات الفطيرة ثنائية/ثلاثية الأبعاد |
| InsideEnd | `2` | ينطبق فقط على المخططات الشريطية |
| OutsideEnd | `3` | ينطبق فقط على المخططات الشريطية ومخططات الفطيرة ثنائية/ثلاثية الأبعاد |
| Above | `4` | ينطبق فقط على المخططات الخطية |
| Below | `5` | ينطبق فقط على المخططات الخطية |
| Left | `6` | ينطبق فقط على المخططات الخطية |
| Right | `7` | ينطبق فقط على المخططات الخطية |
| BestFit | `8` | ينطبق فقط على مخططات الفطيرة ثنائية/ثلاثية الأبعاد |
| Moved | `9` | قام المستخدم بنقل تسميات البيانات. هذا مخصص فقط لقراءة المخطط من ملف القالب. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LabelPositionTypeDemo
    {
        public static void LabelPositionTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات النموذجية للمخطط
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

            // أضف سلسلة البيانات إلى المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى ملصقات البيانات للسلسلة الأولى
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // تعيين موضع تسميات البيانات
            dataLabels.Position = LabelPositionType.InsideBase;

            // إظهار اسم الفئة في تسميات البيانات
            dataLabels.ShowCategoryName = true;

            // إظهار القيمة في تسميات البيانات
            dataLabels.ShowValue = true;

            // احفظ المصنف
            workbook.Save("LabelPositionTypeExample.xlsx");
            workbook.Save("LabelPositionTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


