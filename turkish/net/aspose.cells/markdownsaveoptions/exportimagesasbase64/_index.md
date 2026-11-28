---
title: "MarkdownSaveOptions.ExportImagesAsBase64"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MarkdownSaveOptions özelliği. Görsellerin Base64 biçiminde Markdown'a kaydedilip kaydedilmediğini belirtir. Varsayılan değer true'dur."
type: docs
url: /tr/net/aspose.cells/markdownsaveoptions/exportimagesasbase64/
---
## MarkdownSaveOptions.ExportImagesAsBase64 property

Görsellerin Markdown'a Base64 biçiminde kaydedilip kaydedilmeyeceğini belirtir. Varsayılan değer true'dur.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Açıklamalar

Bu özellik true olarak ayarlandığında, görüntü verileri doğrudan img öğelerine gömülür ve ayrı dosyalar oluşturulmaz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ve bir görsel ekle
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("With Image");

            // Çalışma sayfasına bir resim ekle
            int imageIndex = worksheet.Pictures.Add(1, 1, "sample.png");

            try
            {
                // MarkdownSaveOptions örneği oluştur
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // ExportImagesAsBase64 özelliğinin varsayılan değerini göster
                Console.WriteLine("Default ExportImagesAsBase64 value: " + saveOptions.ExportImagesAsBase64);

                // ExportImagesAsBase64 özelliğini false olarak ayarlayarak özelliği göster
                saveOptions.ExportImagesAsBase64 = false;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // ExportImagesAsBase64 = false ile kaydet
                workbook.Save("MarkdownImagesAsFiles.md", saveOptions);

                // ExportImagesAsBase64 özelliğini true olarak ayarla
                saveOptions.ExportImagesAsBase64 = true;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // ExportImagesAsBase64 = true ile kaydet
                workbook.Save("MarkdownImagesAsBase64.md", saveOptions);

                Console.WriteLine("Markdown files saved with different ExportImagesAsBase64 settings.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


