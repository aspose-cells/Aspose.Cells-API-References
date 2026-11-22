---
title: "Enum PrintSizeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.PrintSizeType enum. يمثل حجم المخطط المطبوع"
type: docs
url: /ar/net/aspose.cells/printsizetype/
---
## PrintSizeType enumeration

يمثل حجم المخطط المطبوع.

```csharp
public enum PrintSizeType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Full | `0` | استخدام الصفحة الكاملة. |
| Fit | `1` | تحجيم لتناسب الصفحة. |
| Custom | `2` | مخصص. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PrintSizeTypeDemo
    {
        public static void PrintSizeTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // احصل على ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تحديد نطاق البيانات للمخطط
            chart.SetChartDataRange("A1:B4", true);

            // تعيين عنوان المخطط
            chart.Title.Text = "Sample Chart";

            // تعيين حجم الطباعة للمخطط
            chart.PrintSize = PrintSizeType.Fit;

            // احفظ المصنف
            workbook.Save("PrintSizeTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


