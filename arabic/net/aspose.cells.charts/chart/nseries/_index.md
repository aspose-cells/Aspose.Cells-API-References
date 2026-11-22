---
title: "Chart.NSeries"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المخطط. تحصل على مجموعة SeriesCollection التي تمثل سلسلة البيانات في المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chart/nseries/
---
## Chart.NSeries property

يحصل على مجموعة [`SeriesCollection`](../../seriescollection/) التي تمثل سلسلة البيانات في المخطط.

```csharp
public SeriesCollection NSeries { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyNSeriesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 2, 25, 11);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

            // حدد مصدر البيانات لسلسلة المخطط باستخدام NSeries
            chart.NSeries.Add("=Sheet1!$A$2:$B$10", true);

            // تعيين عنوان المخطط
            chart.Title.Text = "NSeries Demo Chart";

            // احفظ المصنف
            workbook.Save("NSeriesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


