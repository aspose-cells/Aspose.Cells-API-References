---
title: "TilePicOption.ScaleY"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TilePicOption özelliği. Döşeme resmi için Y ölçeğini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/tilepicoption/scaley/
---
## TilePicOption.ScaleY property

Döşeme resminin Y ölçeğini alır veya ayarlar.

```csharp
public double ScaleY { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TilePicOptionPropertyScaleYDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Görüntü ile doku dolgu ayarla
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            byte[] imageData = File.ReadAllBytes("example.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            
            // ScaleY ile döşeme seçeneklerini yapılandır
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
            
            // Çalışma kitabını kaydedin
            workbook.Save("TilePicOptionScaleYDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


