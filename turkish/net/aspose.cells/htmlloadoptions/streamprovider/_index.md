---
title: "HtmlLoadOptions.StreamProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlLoadOptions özelliği. Nesneleri içe aktarmak için StreamProviderImportHtmlFile'ı alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/htmlloadoptions/streamprovider/
---
## HtmlLoadOptions.StreamProvider property

Nesneleri içe aktarmak için StreamProviderImportHtmlFile'ı alır veya ayarlar.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyStreamProviderDemo : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            // Gerektiği gibi akışı başlatın
        }

        public Stream ProvideStream(StreamProviderOptions options)
        {
            // Okuma/yazma için bir akış döndürün
            return File.Open(options.DefaultPath, FileMode.OpenOrCreate, FileAccess.ReadWrite);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Akimı kapatın
            options.Stream.Close();
        }

        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("StreamProvider Demo");

            // Özel StreamProvider ile kaydedin
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
            workbook.Save("output.html", saveOptions);

            // Özel StreamProvider ile yükleyin
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("output.html", loadOptions);

            // Yüklenen verileri doğrulayın
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


