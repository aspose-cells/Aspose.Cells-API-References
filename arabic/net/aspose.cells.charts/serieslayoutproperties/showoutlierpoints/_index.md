---
title: "SeriesLayoutProperties.ShowOutlierPoints"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SeriesLayoutProperties. تشير إلى ما إذا كانت نقاط البيانات الشاذة معروضة"
type: docs
url: /ar/net/aspose.cells.charts/serieslayoutproperties/showoutlierpoints/
---
## SeriesLayoutProperties.ShowOutlierPoints property

يشير إلى ما إذا كانت نقاط البيانات الشاذة معروضة.

```csharp
public bool ShowOutlierPoints { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowOutlierPointsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(200); // Outlier value
            worksheet.Cells["B1"].PutValue("Q1");
            worksheet.Cells["B2"].PutValue("Q2");
            worksheet.Cells["B3"].PutValue("Q3");
            worksheet.Cells["B4"].PutValue("Q4");

            // إنشاء مخطط عمودي (يدعم نقاط البيانات الشاذة)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.CategoryData = "B1:B4";
            
            // تكوين خصائص SeriesLayoutProperties
            Series series = chart.NSeries[0];
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            
            // توضيح خاصية ShowOutlierPoints
            layoutProperties.ShowOutlierPoints = true;
            layoutProperties.ShowInnerPoints = true;
            layoutProperties.ShowMeanMarker = true;

            workbook.Save("ChartWithOutliers.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


