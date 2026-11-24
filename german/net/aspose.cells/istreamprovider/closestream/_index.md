---
title: "IStreamProvider.CloseStream"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IStreamProvider-Methode. Schließt den Stream"
type: docs
url: /de/net/aspose.cells/istreamprovider/closestream/
---
## IStreamProvider.CloseStream method

Schließt den Stream.

```csharp
public void CloseStream(StreamProviderOptions options)
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

    public class IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo : IStreamProvider
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle eine Instanz der Demo-Klasse, die IStreamProvider implementiert
            var streamProvider = new IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo();
            
            // Erstelle StreamProviderOptions
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "output_files/sheet001.htm",
                Stream = new MemoryStream()
            };

            try
            {
                // Rufe die CloseStream-Methode auf
                streamProvider.CloseStream(options);
                
                Console.WriteLine("CloseStream method executed successfully with StreamProviderOptions");
                
                // Demonstriere die Wirkung – im realen Szenario würde dies den Stream schließen
                Console.WriteLine($"Stream closed status: {options.Stream == null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CloseStream method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("IStreamProviderCloseStreamDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Implementierung, die vom Interface gefordert wird
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

### Siehe auch

* class [StreamProviderOptions](../../streamprovideroptions/)
* interface [IStreamProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


