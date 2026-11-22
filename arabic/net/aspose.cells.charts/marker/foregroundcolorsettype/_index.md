---
title: "Marker.ForegroundColorSetType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Marker. تحصل أو تعين نوع مجموعة لون المقدمة للعلامة"
type: docs
url: /ar/net/aspose.cells.charts/marker/foregroundcolorsettype/
---
## Marker.ForegroundColorSetType property

يحصل أو يضبط نوع مجموعة لون المقدمة للعلامة.

```csharp
public FormattingType ForegroundColorSetType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyForegroundColorSetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة
            chart.NSeries.Add("A1:B3", true);
            
            // تكوين علامة السلسلة
            Series series = chart.NSeries[0];
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;

            workbook.Save("MarkerForegroundColorSetTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FormattingType](../../formattingtype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


