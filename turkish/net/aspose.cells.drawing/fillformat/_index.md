---
title: "FillFormat sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.FillFormat sınıfı. Bir şekil için dolgu biçimlendirmesini temsil eden nesneyi kapsüller."
type: docs
url: /tr/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Bir şekil için doldurma biçimlendirmesini temsil eden nesneyi kapsüller.

```csharp
public class FillFormat
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype/) { get; set; } | Dolgu tipini alır ve ayarlar. |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1/) { get; } | Belirtilen dolgu için gradient renk 1'i döndürür. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2/) { get; } | Belirtilen dolgu için gradient renk 2'yi döndürür. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype/) { get; } | Belirtilen dolgu için gradient renk tipini döndürür. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree/) { get; } | Belirtilen dolgu için gradient derecesini döndürür. Yalnızca Excel 2007 için geçerlidir. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill/) { get; } | Alır [`GradientFill`](./gradientfill/) nesnesini. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle/) { get; } | Belirtilen dolgu için gradient stilini döndürür. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant/) { get; } | Belirtilen dolgu için gradient varyantını döndürür. Yalnızca Excel 2007 için geçerlidir. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata/) { get; set; } | Resim veri bilgisini alır ve ayarlar. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern/) { get; set; } | Bir alanın görüntü desenini temsil eder. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill/) { get; } | Alır [`PatternFill`](./patternfill/) nesnesini. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype/) { get; set; } | Resim formatı tipini alır ve ayarlar. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor/) { get; } | Belirtilen dolgu için gradient ön ayar rengini döndürür. |
| [Scale](../../aspose.cells.drawing/fillformat/scale/) { get; set; } | Resim formatı ölçeğini alır ve ayarlar. |
| [SetType](../../aspose.cells.drawing/fillformat/settype/) { get; set; } | (**Obsolete.**) Alır dolgu formatı ayar türünü. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill/) { get; } | Alır [`SolidFill`](./solidfill/) nesnesini. |
| [Texture](../../aspose.cells.drawing/fillformat/texture/) { get; set; } | Belirtilen dolgu için doku tipini temsil eder. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill/) { get; } | Alır [`TextureFill`](./texturefill/) nesnesini. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency/) { get; set; } | Alan şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [Type](../../aspose.cells.drawing/fillformat/type/) { get; set; } | (**Obsolete.**) Alır ve ayarlar dolgu tipini. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode/)() | Hash kodunu alır. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Belirtilen dolguyu tek renkli bir gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient/)(GradientPresetType, GradientStyleType, int) | Belirtilen dolguyu ön ayarlı renkli bir gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Belirtilen dolguyu iki renkli bir gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Belirtilen dolguyu iki renkli bir gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");
            
            // Çalışma sayfasına bir sütun grafiği ekle
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafiğe veri serisi ekle
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            
            // Seri alanına gradient dolgu uygula
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(System.Drawing.Color.Lime, 1, 
                GradientStyleType.Horizontal, 1);
            
            // Çalışma kitabını kaydedin
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


