---
title: "تعداد TickLabelPositionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.TickLabelPositionType تعداد. يمثل نوع موضع تسميات علامات الفواصل على المحور المحدد"
type: docs
url: /ar/net/aspose.cells.charts/ticklabelpositiontype/
---
## TickLabelPositionType enumeration

يمثل نوع موضع تسميات العلامات على المحور المحدد.

```csharp
public enum TickLabelPositionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| High | `0` | نوع الموضع هو عالي. |
| Low | `1` | نوع الموضع هو منخفض. |
| NextToAxis | `2` | نوع الموضع هو بجوار المحور. |
| None | `3` | نوع الموضع هو لا شيء. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelPositionTypeDemo
    {
        public static void TickLabelPositionTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض البيانات النموذجية إلى ورقة العمل
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
            
            // الوصول إلى محور الفئة
            Axis categoryAxis = chart.CategoryAxis;
            
            // تعيين موضع تسمية الفاصل إلى عالي
            categoryAxis.TickLabelPosition = TickLabelPositionType.High;
            
            // احفظ المصنف
            workbook.Save("TickLabelPositionTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


