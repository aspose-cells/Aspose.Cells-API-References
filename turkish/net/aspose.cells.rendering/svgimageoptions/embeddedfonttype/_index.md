---
title: "SvgImageOptions.EmbeddedFontType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SvgImageOptions özelliği. Svg'ye gömülen yazı tipinin türünü alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/svgimageoptions/embeddedfonttype/
---
## SvgImageOptions.EmbeddedFontType property

Svg'ye gömülen yazı tipi türünü alır veya ayarlar.

```csharp
public SvgEmbeddedFontType EmbeddedFontType { get; set; }
```

### Açıklamalar

Varsayılan değer None'dur ve bu, Svg'ye yazı tipi gömülmeyeceği anlamına gelir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yazı tipi gömülmesini göstermek için özel biçimlendirmeli veri ekle
            var cell = worksheet.Cells["B2"];
            cell.PutValue("SVG Font Embedding Test");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // SVG renderleme seçenekleri oluştur
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // İlk gömülü yazı tipi türünü göster
            Console.WriteLine($"Initial EmbeddedFontType: {svgOptions.EmbeddedFontType}");

            // Çalışma sayfasını yazı tipi gömmeden SVG'ye dönüştür
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "WithoutFontEmbedding.svg");

            // Gömülü yazı tipi türünü WOFF'a değiştir
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

            // Çalışma sayfasını WOFF yazı tipi gömülü olarak SVG'ye dönüştür
            SheetRender renderer2 = new SheetRender(worksheet, svgOptions);
            renderer2.ToImage(0, "WithWoffFontEmbedding.svg");

            Console.WriteLine("Generated SVG files with different font embedding settings.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SvgEmbeddedFontType](../../svgembeddedfonttype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


