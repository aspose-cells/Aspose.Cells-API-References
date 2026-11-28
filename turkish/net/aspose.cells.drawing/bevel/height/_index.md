---
title: "Bevel.Height"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Bevel özelliği. Bevel'in yüksekliğini alır ve ayarlar veya şeklin üzerinde ne kadar yukarı uygulanacağını. Birim olarak Nokta"
type: docs
url: /tr/net/aspose.cells.drawing/bevel/height/
---
## Bevel.Height property

Köşebentin yüksekliğini alır ve ayarlar, ya da şeklin üzerinde ne kadar yukarı uygulandığını. Birim olarak Nokta kullanılır.

```csharp
public double Height { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class BevelPropertyHeightDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(1500);

            // 3D sütun grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Grafik alanının 3D formatına eriş
            Format3D format3D = chart.PlotArea.ShapeProperties.Format3D;

            // Yükseklik özelliğiyle üst bevel'i yapılandır
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.ArtDeco;
            topBevel.Width = 8;
            topBevel.Height = 4.5; // Demonstrating Height property usage

            // Çalışma kitabını kaydedin
            workbook.Save("BevelHeightDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


