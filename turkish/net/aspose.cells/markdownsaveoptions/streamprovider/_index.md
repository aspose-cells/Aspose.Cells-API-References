---
title: "MarkdownSaveOptions.StreamProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MarkdownSaveOptions özelliği. Nesneleri dışa aktarmak için IStreamProvider'ı alır veya ayarlar. Null ise dışa aktarılan nesneler çıktı dosyasıyla aynı dizine kaydedilir."
type: docs
url: /tr/net/aspose.cells/markdownsaveoptions/streamprovider/
---
## MarkdownSaveOptions.StreamProvider property

Nesneleri dışa aktarmak için IStreamProvider'ı alır veya ayarlar. `null` ise, dışa aktarılan nesneler çıktı dosyasıyla aynı dizine kaydedilir.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MarkdownSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].Value = "Hello";
            worksheet.Cells["B1"].Value = "World";

            try
            {
                // MarkdownSaveOptions örneği oluştur
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Mevcut StreamProvider değerini göster (varsayılan olarak null)
                Console.WriteLine("Current StreamProvider: " + (saveOptions.StreamProvider == null ? "null" : "set"));

                // Özel bir StreamProvider uygulaması oluştur
                CustomStreamProvider streamProvider = new CustomStreamProvider();
                saveOptions.StreamProvider = streamProvider;

                // Güncellenmiş StreamProvider değerini göster
                Console.WriteLine("Updated StreamProvider: " + (saveOptions.StreamProvider != null ? "set" : "null"));

                // Çalışma kitabını özel StreamProvider ile kaydet
                workbook.Save("StreamProviderDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved with custom StreamProvider.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    // IStreamProvider'ın özel uygulaması
    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            Console.WriteLine("Initializing stream");
        }

        public void CloseStream(StreamProviderOptions options)
        {
            Console.WriteLine("Closing stream");
        }
    }
}
```

### Ayrıca Bakınız

* interface [IStreamProvider](../../istreamprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


