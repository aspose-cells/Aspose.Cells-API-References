---
title: "Series.DoughnutHoleSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Seri özelliği. Bir halka grafik grubundaki deliğin boyutunu döndürür veya ayarlar. Delik boyutu, grafik boyutunun yüzde 10 ile 90 arasında bir yüzdesi olarak ifade edilir"
type: docs
url: /tr/net/aspose.cells.charts/series/doughnutholesize/
---
## Series.DoughnutHoleSize property

Bir halka grafik grubundaki deliğin boyutunu döndürür veya ayarlar. Delik boyutu, grafik boyutunun yüzde olarak ifade edilir ve %10 ile %90 arasında olur.

```csharp
public int DoughnutHoleSize { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDoughnutHoleSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Bir doughnut grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Halka delik boyutunu ayarlayın (grafik yarıçapının yüzdesi)
            chart.NSeries[0].DoughnutHoleSize = 25;

            // Çalışma kitabını kaydedin
            workbook.Save("DoughnutHoleSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


