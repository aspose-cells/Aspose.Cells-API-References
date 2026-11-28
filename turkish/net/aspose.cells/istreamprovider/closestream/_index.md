---
title: "IStreamProvider.CloseStream"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IStreamProvider metodu. Akışı kapatır"
type: docs
url: /tr/net/aspose.cells/istreamprovider/closestream/
---
## IStreamProvider.CloseStream method

Akışı kapatır.

```csharp
public void CloseStream(StreamProviderOptions options)
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

    public class IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo : IStreamProvider
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // IStreamProvider'ı uygulayan demo sınıfının bir örneğini oluştur
            var streamProvider = new IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo();
            
            // StreamProviderOptions oluştur.
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "output_files/sheet001.htm",
                Stream = new MemoryStream()
            };

            try
            {
                // CloseStream metodunu çağır
                streamProvider.CloseStream(options);
                
                Console.WriteLine("CloseStream method executed successfully with StreamProviderOptions");
                
                // Etkiyi göster - gerçek senaryoda bu akışı kapatır
                Console.WriteLine($"Stream closed status: {options.Stream == null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CloseStream method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("IStreamProviderCloseStreamDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Arayüzün gerektirdiği uygulama
        }

        public void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
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


