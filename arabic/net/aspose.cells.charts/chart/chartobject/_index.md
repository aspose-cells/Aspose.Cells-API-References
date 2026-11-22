---
title: "Chart.ChartObject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تمثل chartShape"
type: docs
url: /ar/net/aspose.cells.charts/chart/chartobject/
---
## Chart.ChartObject property

يمثل الـ chartShape؛

```csharp
public ChartShape ChartObject { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyChartObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // عرض خصائص ChartObject
            chart.ChartObject.Placement = PlacementType.Move;
            chart.ChartObject.X = 100;
            chart.ChartObject.Y = 200;
            chart.ChartObject.Width = 400;
            chart.ChartObject.Height = 300;

            // احفظ المصنف
            workbook.Save("ChartObjectDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [ChartShape](../../../aspose.cells.drawing/chartshape/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


