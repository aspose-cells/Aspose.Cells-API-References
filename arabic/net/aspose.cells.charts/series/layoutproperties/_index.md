---
title: "Series.LayoutProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تمثل خصائص التخطيط"
type: docs
url: /ar/net/aspose.cells.charts/series/layoutproperties/
---
## Series.LayoutProperties property

يمثل خصائص التخطيط.

```csharp
public SeriesLayoutProperties LayoutProperties { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyLayoutPropertiesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // بيانات عينة لمخطط الصندوق والشارب
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Q1");
            sheet.Cells["A3"].PutValue("Q1");
            sheet.Cells["A4"].PutValue("Q1");
            sheet.Cells["A5"].PutValue("Q2");
            sheet.Cells["A6"].PutValue("Q2");
            sheet.Cells["A7"].PutValue("Q2");

            sheet.Cells["B1"].PutValue("Series1");
            sheet.Cells["B2"].PutValue(15);
            sheet.Cells["B3"].PutValue(25);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(20);
            sheet.Cells["B6"].PutValue(35);
            sheet.Cells["B7"].PutValue(40);

            // أضف مخطط الصندوق والشارب
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.BoxWhisker, 5, 0, 25, 10);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("B1:B7", true);
            chart.NSeries.CategoryData = "A2:A7";

            // تكوين خصائص التخطيط للسلسلة
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.LayoutProperties.ShowMeanLine = false;
            series.LayoutProperties.ShowInnerPoints = true;
            series.LayoutProperties.ShowOutlierPoints = true;
            series.LayoutProperties.ShowMeanMarker = true;

            // احفظ المصنف
            workbook.Save("SeriesLayoutPropertiesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesLayoutProperties](../../serieslayoutproperties/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


