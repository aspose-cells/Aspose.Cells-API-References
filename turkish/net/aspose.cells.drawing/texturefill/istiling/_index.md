---
title: "TextureFill.IsTiling"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextureFill özelliği. Resmin doku olarak döşenip döşenmediğini gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/texturefill/istiling/
---
## TextureFill.IsTiling property

Resmin doku olarak döşenip döşenmediğini gösterir.

```csharp
public bool IsTiling { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextureFillPropertyIsTilingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik verilerini ayarla
            chart.NSeries.Add("A1:B3", true);
            
            // Grafik alanı için doku doldurmayı ayarla
            chart.PlotArea.Area.FillFormat.Texture = TextureType.BlueTissuePaper;
            
            // IsTiling özelliğini ayarla
            chart.PlotArea.Area.FillFormat.TextureFill.IsTiling = true;
            
            // IsTiling değerini doğrula ve çıktısını al
            Console.WriteLine("IsTiling: " + chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
            
            // Çalışma kitabını kaydedin
            workbook.Save("TextureFillIsTilingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


