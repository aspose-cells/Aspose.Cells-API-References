---
title: "IStreamProvider.InitStream"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IStreamProvider-metod. Hämtar strömmen"
type: docs
url: /sv/net/aspose.cells/istreamprovider/initstream/
---
## IStreamProvider.InitStream method

Hämtar strömmen.

```csharp
public void InitStream(StreamProviderOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | StreamProviderOptions |  |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en instans av demoklassen som implementerar IStreamProvider
            var streamProvider = new IStreamProviderMethodInitStreamWithStreamProviderOptionsDemo();
            
            // Förbered StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "custom_path",
                Stream = new MemoryStream()
            };

            try
            {
                // Anropa InitStream-metoden med StreamProviderOptions-parameter
                streamProvider.InitStream(options);
                
                Console.WriteLine("InitStream method executed successfully with StreamProviderOptions parameter");
                
                // Demonstrera effekten – i det här fallet visar vi bara att strömmen är initierad
                Console.WriteLine($"Stream initialized: {options.Stream != null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InitStream method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("MethodInitStreamWithStreamProviderOptionsDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Implementering av InitStream
            Console.WriteLine($"Initializing stream with ResourceLoadingType: {options.ResourceLoadingType}");
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Implementering av CloseStream
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }
    }
}
```

### Se även

* class [StreamProviderOptions](../../streamprovideroptions/)
* interface [IStreamProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


