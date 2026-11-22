---
title: "Marker.MarkerStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Marker. تمثل نمط العلامة. تنطبق على مخطط الخط ومخطط التبعثر أو مخطط الرادار"
type: docs
url: /ar/net/aspose.cells.charts/marker/markerstyle/
---
## Marker.MarkerStyle property

يمثل نمط العلامة. ينطبق على مخطط خط، مخطط مبعثر، أو مخطط رادار.

```csharp
public ChartMarkerType MarkerStyle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["B4"].PutValue(6);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // تعيين نمط العلامة للسلسلة الأولى
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Circle;
            chart.NSeries[0].Marker.ForegroundColor = System.Drawing.Color.Blue;
            chart.NSeries[0].Marker.BackgroundColor = System.Drawing.Color.White;
            chart.NSeries[0].Marker.MarkerSize = 10;

            // احفظ المصنف
            workbook.Save("MarkerStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ChartMarkerType](../../chartmarkertype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


