---
title: "IStreamProvider arayüzü"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.IStreamProvider arayüzü. Dışa aktarılan akış sağlayıcısını temsil eder"
type: docs
url: /tr/net/aspose.cells/istreamprovider/
---
## IStreamProvider interface

Dışa aktarılan akış sağlayıcısını temsil eder.

```csharp
public interface IStreamProvider
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CloseStream](../../aspose.cells/istreamprovider/closestream/)(StreamProviderOptions) | Akışı kapatır. |
| [InitStream](../../aspose.cells/istreamprovider/initstream/)(StreamProviderOptions) | Akışı alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IStreamProviderDemo : IStreamProvider
    {
        // InitStream metodunu uygulama
        public void InitStream(StreamProviderOptions options)
        {
            string outputDir = "/test/";
            string path = outputDir + Path.GetFileName(options.DefaultPath);
            options.CustomPath = path;
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
        }

        // CloseStream metodunu uygulama
        public void CloseStream(StreamProviderOptions options)
        {
            // Akış null değilse kapat
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }

        public static void IStreamProviderExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı verileri ayarla
            worksheet.Cells["A1"].PutValue("Hello World");

            // HtmlSaveOptions oluşturun ve StreamProvider'ı ayarlayın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new IStreamProviderDemo();

            // Çalışma kitabını HTML formatında kaydedin
            workbook.Save("IStreamProviderExample.html", saveOptions);

            // Çalışma kitabını HTML formatından yükleyin
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new IStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("IStreamProviderExample.html", loadOptions);

            // Yüklenen verileri görüntüleyin
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }

}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


