---
title: "IStreamProvider.InitStream"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IStreamProvider yöntemi. Akışı alır"
type: docs
url: /tr/net/aspose.cells/istreamprovider/initstream/
---
## IStreamProvider.InitStream method

Akışı alır.

```csharp
public void InitStream(StreamProviderOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | StreamProviderOptions |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IStreamProviderMethodInitStreamWithStreamProviderOptionsDemo : IStreamProvider
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // IStreamProvider'ı uygulayan demo sınıfının bir örneğini oluştur
            var streamProvider = new IStreamProviderMethodInitStreamWithStreamProviderOptionsDemo();
            
            // StreamProviderOptions'ı Hazırla
            StreamProviderOptions options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "custom_path",
                Stream = new MemoryStream()
            };

            try
            {
                // InitStream metodunu StreamProviderOptions parametresiyle çağır
                streamProvider.InitStream(options);
                
                Console.WriteLine("InitStream method executed successfully with StreamProviderOptions parameter");
                
                // Etkiyi göster - bu durumda yalnızca akışın başlatıldığını gösteriyoruz
                Console.WriteLine($"Stream initialized: {options.Stream != null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InitStream method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("MethodInitStreamWithStreamProviderOptionsDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // InitStream'in uygulanması
            Console.WriteLine($"Initializing stream with ResourceLoadingType: {options.ResourceLoadingType}");
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // CloseStream'in uygulanması
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [StreamProviderOptions](../../streamprovideroptions/)
* interface [IStreamProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


