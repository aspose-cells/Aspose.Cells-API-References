---
title: "Axis.AxisLine"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. Bir eksenin görünümünü alır"
type: docs
url: /tr/net/aspose.cells.charts/axis/axisline/
---
## Axis.AxisLine property

Bir eksenin görünümünü alır.

```csharp
public Line AxisLine { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAxisLineDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Değer eksenine erişin
            Axis valueAxis = chart.ValueAxis;

            // Eksen çizgi özelliklerini özelleştir
            valueAxis.AxisLine.Color = Color.Red;
            valueAxis.AxisLine.Style = LineType.DashDot;
            valueAxis.AxisLine.Weight = WeightType.MediumLine;

            // Çalışma kitabını kaydedin
            workbook.Save("AxisLineDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


