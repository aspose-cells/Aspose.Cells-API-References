---
title: "Series.FirstSliceAngle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تحصل أو تعين زاوية الشريحة الأولى في مخطط الفطيرة أو مخطط الدونات بالدرجات باتجاه عقارب الساعة من العمودي. ينطبق فقط على مخططات الفطيرة، الفطيرة ثلاثية الأبعاد، والدونات بقيم من 0 إلى 360"
type: docs
url: /ar/net/aspose.cells.charts/series/firstsliceangle/
---
## Series.FirstSliceAngle property

يحصل على أو يضبط زاوية الشريحة الأولى في مخطط الفطيرة أو مخطط الدونات، بالدرجات (مع اتجاه عقارب الساعة من العمودي). ينطبق فقط على مخططات الفطيرة، الفطيرة ثلاثية الأبعاد، ومخططات الدونات، بقيم من 0 إلى 360.

```csharp
public short FirstSliceAngle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة لمخطط الفطيرة
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // أضف مخططًا دائريًا
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على السلسلة الأولى وعين FirstSliceAngle
            Series series = chart.NSeries[0];
            series.FirstSliceAngle = 45; // Rotate pie chart by 45 degrees

            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


