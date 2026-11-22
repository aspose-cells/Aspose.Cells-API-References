---
title: "Chart.FilteredNSeries"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تحصل على مجموعة SeriesCollection تمثل سلاسل البيانات التي تم تصفيتها في المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chart/filterednseries/
---
## Chart.FilteredNSeries property

تحصل على مجموعة [`SeriesCollection`](../../seriescollection/) تمثل سلاسل البيانات التي تم تصفيتها في المخطط.

```csharp
public SeriesCollection FilteredNSeries { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFilteredNSeriesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Series 1");
            worksheet.Cells["A3"].PutValue("Series 2");
            worksheet.Cells["A4"].PutValue("Series 3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط وتعيين بعض السلاسل كمرشحة
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تصفية بعض السلاسل (إخفاء السلسلة 2)
            chart.NSeries[1].IsFiltered = true;

            // الوصول إلى مجموعة السلاسل المصفاة
            Aspose.Cells.Charts.SeriesCollection filteredSeries = chart.FilteredNSeries;
            Console.WriteLine("Filtered Series Count: " + filteredSeries.Count.ToString());

            // احفظ المصنف
            workbook.Save("FilteredNSeriesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


