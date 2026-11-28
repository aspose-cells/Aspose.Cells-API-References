---
title: "ChartArea.Height"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartArea özelliği. Grafik alanının alt sağ köşe satırından dikey ofseti, grafik alanının 1/4000 biriminde alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartarea/height/
---
## ChartArea.Height property

Alt‑sağ köşe satırından dikey ofseti, grafik alanının 1/4000 biriminde alır veya ayarlar.

```csharp
[Obsolete("Use ChartArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ChartArea.HeightRatioToChart özelliğini kullanın. Yükseklik = HeightRatioToChart * 4000. Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyHeightDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafik alanına eriş
            ChartArea chartArea = chart.ChartArea;

            // Height özelliğini göster
            Console.WriteLine("Original Chart Area Height: " + chartArea.Height);
            
            // Yüksekliği değiştir
            chartArea.Height = 500;
            Console.WriteLine("Modified Chart Area Height: " + chartArea.Height);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartAreaHeightDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


