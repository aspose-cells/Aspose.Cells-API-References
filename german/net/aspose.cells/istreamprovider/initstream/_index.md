---
title: "IStreamProvider.InitStream"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IStreamProvider-Methode. Ruft den Stream ab"
type: docs
url: /de/net/aspose.cells/istreamprovider/initstream/
---
## IStreamProvider.InitStream method

Liest den Stream.

```csharp
public void InitStream(StreamProviderOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | StreamProviderOptions |  |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle eine Instanz der Demo-Klasse, die IStreamProvider implementiert
            var streamProvider = new IStreamProviderMethodInitStreamWithStreamProviderOptionsDemo();
            
            // Bereite StreamProviderOptions vor
            StreamProviderOptions options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "custom_path",
                Stream = new MemoryStream()
            };

            try
            {
                // Rufe die InitStream-Methode mit dem Parameter StreamProviderOptions auf
                streamProvider.InitStream(options);
                
                Console.WriteLine("InitStream method executed successfully with StreamProviderOptions parameter");
                
                // Demonstriere die Wirkung – in diesem Fall zeigen wir nur, dass der Stream initialisiert ist
                Console.WriteLine($"Stream initialized: {options.Stream != null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InitStream method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("MethodInitStreamWithStreamProviderOptionsDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Implementierung von InitStream
            Console.WriteLine($"Initializing stream with ResourceLoadingType: {options.ResourceLoadingType}");
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Implementierung von CloseStream
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }
    }
}
```

### Siehe auch

* class [StreamProviderOptions](../../streamprovideroptions/)
* interface [IStreamProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


