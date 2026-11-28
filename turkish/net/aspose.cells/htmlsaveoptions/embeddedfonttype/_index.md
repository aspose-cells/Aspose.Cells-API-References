---
title: "HtmlSaveOptions.EmbeddedFontType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. HTML dosyasına gömülecek font dosyasının türünü alır veya ayarlar. Varsayılan değer None'dur ve bu, HTML'e font gömülmeyeceği anlamına gelir."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/embeddedfonttype/
---
## HtmlSaveOptions.EmbeddedFontType property

Yazı tipi dosyasının HTML dosyasına gömülme türünü alır veya ayarlar. Varsayılan değer None'dır ve bu, HTML'ye yazı tipi gömülmeyeceği anlamına gelir.

```csharp
public HtmlEmbeddedFontType EmbeddedFontType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Sample Text with Font");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);

            try
            {
                // HTML kaydetme seçenekleri oluştur
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Varsayılan EmbeddedFontType değerini gösterin
                Console.WriteLine("Default EmbeddedFontType: " + options.EmbeddedFontType);

                // EmbeddedFontType'ı Woff olarak ayarlayın
                options.EmbeddedFontType = HtmlEmbeddedFontType.Woff;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Çalışma kitabını WOFF font gömme ile kaydedin
                workbook.Save("EmbeddedFontType_Woff.html", options);

                // None olarak sıfırlayın
                options.EmbeddedFontType = HtmlEmbeddedFontType.None;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Çalışma kitabını font gömmeden kaydedin
                workbook.Save("EmbeddedFontType_None.html", options);

                Console.WriteLine("EmbeddedFontType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [HtmlEmbeddedFontType](../../../aspose.cells.rendering/htmlembeddedfonttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


