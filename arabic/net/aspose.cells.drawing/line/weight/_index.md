---
title: "Line.Weight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخط. تحصل أو تعيين WeightType للخط"
type: docs
url: /ar/net/aspose.cells.drawing/line/weight/
---
## Line.Weight property

تحصل أو تعيين [`WeightType`](../../weighttype/) للخط.

```csharp
public WeightType Weight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightDemo
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

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى منطقة المخطط وضبط وزن الحدود
            ChartArea chartArea = chart.ChartArea;
            chartArea.Border.Weight = WeightType.MediumLine;

            // احفظ المصنف
            workbook.Save("LinePropertyWeightDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* enum [WeightType](../../weighttype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


