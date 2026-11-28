---
title: "Sınıf TilePicOption"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.TilePicOption sınıfı. Döşeme resmini doku olarak temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/tilepicoption/
---
## TilePicOption class

Döşeme resmini doku olarak temsil eder.

```csharp
public class TilePicOption
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [TilePicOption](tilepicoption/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing/tilepicoption/alignmenttype/) { get; set; } | Döşeme hizalamasını alır veya ayarlar. |
| [MirrorType](../../aspose.cells.drawing/tilepicoption/mirrortype/) { get; set; } | Döşeme için ayna tipini alır veya ayarlar. |
| [OffsetX](../../aspose.cells.drawing/tilepicoption/offsetx/) { get; set; } | Döşeme resminin X ofsetini alır veya ayarlar. |
| [OffsetY](../../aspose.cells.drawing/tilepicoption/offsety/) { get; set; } | Döşeme resminin Y ofsetini alır veya ayarlar. |
| [ScaleX](../../aspose.cells.drawing/tilepicoption/scalex/) { get; set; } | Döşeme resminin X ölçeğini alır veya ayarlar. |
| [ScaleY](../../aspose.cells.drawing/tilepicoption/scaley/) { get; set; } | Döşeme resminin Y ölçeğini alır veya ayarlar. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTilePicOptionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gösterim için bir grafik ekle
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Dolgu tipini doku olarak ayarla
            chart.ChartArea.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Texture;

            // Örnek resmi yükle (gerçek yol ile değiştir)
            byte[] imageData = File.ReadAllBytes("sample.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // TilePicOption oluştur ve yapılandır
            TilePicOption tileOptions = new TilePicOption();
            tileOptions.ScaleX = 50;
            tileOptions.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = tileOptions;

            // Çalışma kitabını kaydedin
            workbook.Save("TilePicOptionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


