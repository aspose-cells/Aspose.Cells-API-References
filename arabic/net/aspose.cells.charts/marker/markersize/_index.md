---
title: "Marker.MarkerSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Marker. تمثل حجم العلامة بوحدة النقاط. تنطبق على مخطط الخط ومخطط التبعثر أو مخطط الرادار"
type: docs
url: /ar/net/aspose.cells.charts/marker/markersize/
---
## Marker.MarkerSize property

يمثل حجم العلامة بوحدة النقاط. ينطبق على مخطط خط، مخطط مبعثر، أو مخطط رادار.

```csharp
public int MarkerSize { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i + 1);
                worksheet.Cells[i + 1, 1].PutValue((i + 1) * 2);
            }

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة سلسلة - استدعاء الطريقة المصحح
            int seriesIndex = chart.NSeries.Add("B2:B11", true);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A11";

            // تعيين خصائص العلامة
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Demonstrating MarkerSize property
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.BackgroundColor = Color.Yellow;

            // احفظ المصنف
            workbook.Save("MarkerSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


