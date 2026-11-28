---
title: "Axis.TickLabelSpacing"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. İşaretleme etiketi arasındaki kategori veya seri sayısını temsil eder. Yalnızca kategori ve seri eksenlerine uygulanır."
type: docs
url: /tr/net/aspose.cells.charts/axis/ticklabelspacing/
---
## Axis.TickLabelSpacing property

İşaretleme etiketleri arasındaki kategori veya seri sayısını temsil eder. Yalnızca kategori ve seri eksenlerine uygulanır.

```csharp
public int TickLabelSpacing { get; set; }
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
    public class AxisPropertyTickLabelSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik verilerini ayarla
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Eksen işaretleme etiketi aralığını yapılandır
            chart.CategoryAxis.TickLabelSpacing = 2; // Show every 2nd label

            workbook.Save("AxisPropertyTickLabelSpacingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


