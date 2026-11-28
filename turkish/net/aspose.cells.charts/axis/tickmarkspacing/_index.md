---
title: "Axis.TickMarkSpacing"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. İşaretçiler arasındaki kategori veya seri sayısını döndürür veya ayarlar. Yalnızca kategori ve seri eksenlerine uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/axis/tickmarkspacing/
---
## Axis.TickMarkSpacing property

İşaretler arasındaki kategori veya seri sayısını döndürür veya ayarlar. Yalnızca kategori ve seri eksenlerine uygulanır.

```csharp
public int TickMarkSpacing { get; set; }
```

### Açıklamalar

Sayı 1 ile 31999 arasında olmalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickMarkSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // TickMarkSpacing ile değer eksenini yapılandır
            Axis valueAxis = chart.ValueAxis;
            valueAxis.MinValue = 0;
            valueAxis.MaxValue = 200;
            valueAxis.MajorUnit = 25;
            valueAxis.MinorUnit = 5;
            valueAxis.TickMarkSpacing = 2; // Setting tick mark spacing
            
            // TickMarkSpacing ile kategori eksenini yapılandır
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.TickMarkSpacing = 1; // Setting tick mark spacing

            workbook.Save("AxisTickMarkSpacingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


