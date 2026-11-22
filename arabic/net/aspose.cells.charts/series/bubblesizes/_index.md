---
title: "Series.BubbleSizes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تحصل أو تعين قيم حجم الفقاعات لسلسلة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/series/bubblesizes/
---
## Series.BubbleSizes property

يحصل أو يحدد قيم حجم الفقاعات لسلسلة المخطط.

```csharp
public string BubbleSizes { get; set; }
```

### ملاحظات

فقط لـ Bubble أو Bubble3D.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleSizesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لمخطط الفقاعات
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["C1"].PutValue("Bubble Sizes");
            
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
                worksheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // إضافة مخطط فقاعات
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Bubble, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // تعيين بيانات السلسلة باستخدام خاصية BubbleSizes
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";
            chart.NSeries[0].BubbleSizes = "C2:C5";

            // احفظ المصنف
            workbook.Save("BubbleChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


