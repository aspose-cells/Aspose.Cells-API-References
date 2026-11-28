---
title: "Chart.Style"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Yerleşik stili alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chart/style/
---
## Chart.Style property

Yerleşik stili alır ve ayarlar.

```csharp
public int Style { get; set; }
```

### Açıklamalar

1 ile 48 arasında olmalıdır. Ayarlanmamışsa -1 döndürün.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart1 = worksheet.Charts[chartIndex];
            chart1.NSeries.Add("B2:B4", false);
            chart1.NSeries.CategoryData = "A2:A4";

            // Başka bir grafik oluştur ve stilini ilk grafikten kopyala
            chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 10, 20, 18);
            Aspose.Cells.Charts.Chart chart2 = worksheet.Charts[chartIndex];
            chart2.NSeries.Add("B2:B4", false);
            chart2.NSeries.CategoryData = "A2:A4";
            
            // Style özelliği kullanımını göster
            chart2.Style = chart1.Style;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


