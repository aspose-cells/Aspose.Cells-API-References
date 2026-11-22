---
title: "Marker.BackgroundColorSetType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Marker. تحصل أو تعين نوع مجموعة لون خلفية العلامة"
type: docs
url: /ar/net/aspose.cells.charts/marker/backgroundcolorsettype/
---
## Marker.BackgroundColorSetType property

يحصل على أو يعيّن نوع مجموعة لون خلفية العلامة.

```csharp
public FormattingType BackgroundColorSetType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyBackgroundColorSetTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
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
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            Series series = chart.NSeries[seriesIndex];

            // تكوين خصائص العلامة
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;
            series.Marker.BackgroundColor = System.Drawing.Color.Yellow;

            // احفظ المصنف
            workbook.Save("MarkerBackgroundColorSetTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FormattingType](../../formattingtype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


