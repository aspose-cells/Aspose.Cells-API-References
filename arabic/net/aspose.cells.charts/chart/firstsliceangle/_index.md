---
title: "Chart.FirstSliceAngle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. يحصل أو يضبط زاوية الشريحة الأولى للمخطط piechart أو doughnutchart بالدرجات باتجاه عقارب الساعة من العمودي. ينطبق فقط على مخططات pie 3D pie و doughnut من 0 إلى 360"
type: docs
url: /ar/net/aspose.cells.charts/chart/firstsliceangle/
---
## Chart.FirstSliceAngle property

يحصل أو يعيّن زاوية الشريحة الأولى في مخطط الفطيرة أو مخطط الدونات، بالدرجات (مع اتجاه عقارب الساعة من العمودي). ينطبق فقط على مخططات الفطيرة، الفطيرة ثلاثية الأبعاد، ومخططات الدونات، من 0 إلى 360.

```csharp
public int FirstSliceAngle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // أضف مخططًا دائريًا
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // حدد نطاق البيانات
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // حدد زاوية الشريحة الأولى إلى 45 درجة
            chart.FirstSliceAngle = 45;
            
            // احفظ المصنف
            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


