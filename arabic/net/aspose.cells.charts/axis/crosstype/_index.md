---
title: "Axis.CrossType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تمثل CrossType على المحور المحدد حيث يعبر المحور الآخر"
type: docs
url: /ar/net/aspose.cells.charts/axis/crosstype/
---
## Axis.CrossType property

تمثل `CrossType` على المحور المحدد حيث يعبر المحور الآخر.

```csharp
public CrossType CrossType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCrossTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // قم بتكوين محور القيم
            chart.ValueAxis.MaxValue = 200;
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MajorUnit = 25;
            
            // إظهار خاصية CrossType
            chart.ValueAxis.CrossType = CrossType.Maximum;

            workbook.Save("AxisPropertyCrossTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CrossType](../../crosstype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


