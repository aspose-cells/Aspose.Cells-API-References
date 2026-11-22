---
title: "Area.InvertIfNegative"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Area. إذا كانت الخاصية true وكانت قيمة نقطة المخطط رقمًا سالبًا، سيتم تبادل لون المقدمة ولون الخلفية"
type: docs
url: /ar/net/aspose.cells.drawing/area/invertifnegative/
---
## Area.InvertIfNegative property

إذا كانت الخاصية صحيحة وكانت قيمة نقطة المخطط عددًا سالبًا، سيتم تبادل لون المقدمة ولون الخلفية.

```csharp
public bool InvertIfNegative { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyInvertIfNegativeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات نموذجية ذات قيمة سلبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            
            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة بيانات وتكوين خصائص المنطقة
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries[0].Area.InvertIfNegative = true;
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.BackgroundColor = Color.Yellow;
            
            workbook.Save("AreaPropertyInvertIfNegativeDemo.xls");
        }
    }
}
```

### انظر أيضًا

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


