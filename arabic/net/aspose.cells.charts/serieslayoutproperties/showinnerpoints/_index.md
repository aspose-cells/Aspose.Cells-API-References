---
title: "SeriesLayoutProperties.ShowInnerPoints"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SeriesLayoutProperties. تشير إلى ما إذا كان يجب إظهار نقاط البيانات غير الشاذة"
type: docs
url: /ar/net/aspose.cells.charts/serieslayoutproperties/showinnerpoints/
---
## SeriesLayoutProperties.ShowInnerPoints property

يشير إلى ما إذا كان يجب إظهار نقاط البيانات غير الشاذة.

```csharp
public bool ShowInnerPoints { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowInnerPointsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لمخطط الصندوق والشارب
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(40);
            worksheet.Cells["A4"].PutValue(15);
            worksheet.Cells["A5"].PutValue(20);
            worksheet.Cells["A6"].PutValue(25);
            worksheet.Cells["A7"].PutValue(30);
            worksheet.Cells["A8"].PutValue(35);
            worksheet.Cells["A9"].PutValue(40);
            worksheet.Cells["A10"].PutValue(45);
            worksheet.Cells["A11"].PutValue(50);

            // أضف مخطط الصندوق والشارب
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة إلى المخطط
            chart.NSeries.Add("A2:A11", true);
            Series series = chart.NSeries[0];

            // تعيين خصائص تخطيط السلسلة
            SeriesLayoutProperties layout = series.LayoutProperties;
            layout.ShowInnerPoints = true; // Demonstrate ShowInnerPoints property
            layout.ShowOutlierPoints = true;
            layout.ShowMeanMarker = true;

            // حساب المخطط
            chart.Calculate();

            // احفظ المصنف
            workbook.Save("BoxWhiskerChart_ShowInnerPoints.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


