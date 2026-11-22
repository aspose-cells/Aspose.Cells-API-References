---
title: "Series.XValues"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تمثل قيم X لهذه السلسلة في المخطط"
type: docs
url: /ar/net/aspose.cells.charts/series/xvalues/
---
## Series.XValues property

يمثل قيم X لهذه السلسلة في المخطط.

```csharp
public string XValues { get; set; }
```

### ملاحظات

فقط لمخطط Scatter و Bubble. يرجى استخدام [`CategoryData`](../../seriescollection/categorydata/) للأنواع الأخرى من المخططات. يتم استخدام [`CategoryValues`](../categoryvalues/) للحصول على القيم الفئوية الفعلية لهذه السلسلة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            var workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i+1, 0].PutValue(i+1); // X values 1-5
                worksheet.Cells[i+1, 1].PutValue((i+1)*2); // Series 1 values
                worksheet.Cells[i+1, 2].PutValue((i+1)*3); // Series 2 values
            }

            // أضف مخطط scatter
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // أضف سلسلة باستخدام XValues و Values
            int seriesIndex = chart.NSeries.Add("B2:B6", false);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property
            series.Name = "Series 1";

            seriesIndex = chart.NSeries.Add("C2:C6", false);
            series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property again
            series.Name = "Series 2";

            // احفظ المصنف
            workbook.Save("SeriesXValuesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


