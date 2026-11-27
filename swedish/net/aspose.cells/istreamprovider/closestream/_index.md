---
title: "IStreamProvider.CloseStream"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IStreamProvider-metod. Stänger strömmen"
type: docs
url: /sv/net/aspose.cells/istreamprovider/closestream/
---
## IStreamProvider.CloseStream method

Stänger strömmen.

```csharp
public void CloseStream(StreamProviderOptions options)
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

    public class IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo : IStreamProvider
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en instans av demoklassen som implementerar IStreamProvider
            var streamProvider = new IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo();
            
            // Skapa StreamProviderOptions
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "output_files/sheet001.htm",
                Stream = new MemoryStream()
            };

            try
            {
                // Anropa CloseStream-metoden
                streamProvider.CloseStream(options);
                
                Console.WriteLine("CloseStream method executed successfully with StreamProviderOptions");
                
                // Demonstrera effekten – i ett verkligt scenario skulle detta stänga strömmen
                Console.WriteLine($"Stream closed status: {options.Stream == null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CloseStream method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("IStreamProviderCloseStreamDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Implementering som krävs av gränssnittet
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

### Se även

* class [StreamProviderOptions](../../streamprovideroptions/)
* interface [IStreamProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


