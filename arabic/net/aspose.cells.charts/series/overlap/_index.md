---
title: "Series.Overlap"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تحدد كيفية تموضع الأشرطة والأعمدة. يمكن أن تكون قيمة بين 100 و 100. ينطبق فقط على مخططات الأشرطة والأعمدة ثنائية الأبعاد"
type: docs
url: /ar/net/aspose.cells.charts/series/overlap/
---
## Series.Overlap property

يحدد كيفية تموضع الأشرطة والأعمدة. يمكن أن تكون قيمة بين -100 و100. ينطبق فقط على مخططات الأشرطة ثنائية الأبعاد ومخططات الأعمدة ثنائية الأبعاد.

```csharp
public short Overlap { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyOverlapDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Series1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["C1"].PutValue("Series2");
            sheet.Cells["C2"].PutValue(15);
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["C4"].PutValue(35);

            // أضف مخطط أعمدة مجمع
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين خاصية التداخل للسلسلة الأولى
            chart.NSeries[0].Overlap = -40;

            // احفظ المصنف
            workbook.Save("SeriesOverlapDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


