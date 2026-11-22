---
title: "Series.IsColorVaried"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تمثل ما إذا كان لون النقاط متنوعًا. يجب أن يحتوي المخطط على سلسلة واحدة فقط أو أن يكون هذا المخطط مخططًا دائريًا"
type: docs
url: /ar/net/aspose.cells.charts/series/iscolorvaried/
---
## Series.IsColorVaried property

يمثل ما إذا كان لون النقاط متنوعًا. يجب أن يحتوي المخطط على سلسلة واحدة فقط أو أن يكون هذا المخطط مخطط فطيرة.

```csharp
public bool IsColorVaried { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsColorVariedDemo
    {
        public static void Run()
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

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين خاصية IsColorVaried للسلسلة الأولى
            chart.NSeries[0].IsColorVaried = true;

            // احفظ المصنف
            workbook.Save("output.xlsx");

            // تحقق من الخاصية
            Console.WriteLine("IsColorVaried: " + chart.NSeries[0].IsColorVaried);
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


