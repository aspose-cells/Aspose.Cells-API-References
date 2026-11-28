---
title: "TextureFill.ImageData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextureFill özelliği. Doldurmanın görüntü verilerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/texturefill/imagedata/
---
## TextureFill.ImageData property

Dolgunun görüntü verisini alır ve ayarlar.

```csharp
public byte[] ImageData { get; set; }
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
    public class TextureFillPropertyImageDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Doku doldurma tipini ayarla
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;

            // Görüntü verisini yükle
            byte[] imageData = File.ReadAllBytes("texture.png");

            // Doku doldurma için görüntü verisini ayarla
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Çalışma kitabını kaydedin
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


