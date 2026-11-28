---
title: "StreamProviderOptions.CustomPath"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StreamProviderOptions özelliği. Kullanıcı tarafından belirlenen özel pathURL, başvurulan kaynağın oluşturulan html dosyasında kaydedilir. Kullanıcı tanımlamazsa DefaultPath kullanılacaktır. Örneğin, sayfa verileri kullanıcı tarafından d/sheet001.htm konumuna kaydedilecek ve ana html dosyasında kullanılan url d/sheet001.htm ya da ana html dosyası tarafından erişilebilecek başka geçerli bir göreli yol olmalıdır."
type: docs
url: /tr/net/aspose.cells/streamprovideroptions/custompath/
---
## StreamProviderOptions.CustomPath property

Kullanıcının özelleştirilmiş yolu (URL), başvurulan kaynak için oluşturulan html dosyasında kaydedilir. Kullanıcı tarafından tanımlanmazsa, DefaultPath kullanılacaktır. Örneğin, sayfa verileri kullanıcı tarafından d:/sheet001.htm konumuna kaydedilecek, ana html dosyasında kullanılan url "d:/sheet001.htm" ya da ana html dosyası tarafından erişilebilen başka geçerli bir göreli yol olmalıdır.

```csharp
public string CustomPath { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyCustomPathDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Özel akış sağlayıcı ile HTML kaydetme seçeneklerini ayarla
            string outputDir = "output";
            Directory.CreateDirectory(outputDir);
            
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
            
            // CustomPath ile özel akış sağlayıcı oluştur
            HtmlWithExternalResourcesProvider streamProvider = new HtmlWithExternalResourcesProvider(outputDir);
            streamProvider.streamProviderOptions.CustomPath = "resources";
            options.StreamProvider = streamProvider;

            // Çalışma kitabını kaydedin
            string outputFile = Path.Combine(outputDir, "output.html");
            workbook.Save(outputFile, options);

            // Özel yolun kullanıldığını doğrula
            string resourcePath = Path.Combine(outputDir, streamProvider.streamProviderOptions.CustomPath);
            Console.WriteLine($"Resources should be saved to: {resourcePath}");
        }
    }

    // Basitleştirilmiş özel akış sağlayıcı uygulaması
    public class HtmlWithExternalResourcesProvider : IStreamProvider
    {
        public StreamProviderOptions streamProviderOptions = new StreamProviderOptions();
        public string _outputDirectory;

        public HtmlWithExternalResourcesProvider(string outputDirectory)
        {
            _outputDirectory = outputDirectory;
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Uygulama burada yer alır
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Uygulama burada yer alır
        }
    }
}
```

### Ayrıca Bakınız

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


