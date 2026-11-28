---
title: "Bevel.Width"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Bevel özelliği. Bevel'in genişliğini alır ve ayarlar veya şekle ne kadar derine uygulanacağını. Birim olarak Nokta"
type: docs
url: /tr/net/aspose.cells.drawing/bevel/width/
---
## Bevel.Width property

Köşebentin genişliğini alır ve ayarlar, ya da şeklin içine ne kadar derine uygulandığını. Birim olarak Nokta kullanılır.

```csharp
public double Width { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class BevelPropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seriyi al ve 3D formatını ayarla
            Series series = chart.NSeries[0];
            Format3D format3D = series.ShapeProperties.Format3D;
            
            // Genişlik gösterimiyle bevel özelliklerini yapılandır
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Width = 12; // Demonstrating Width property
            topBevel.Height = 6;

            // Çalışma kitabını kaydedin
            workbook.Save("BevelWidthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


