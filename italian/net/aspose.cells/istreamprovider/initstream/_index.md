---
title: "IStreamProvider.InitStream"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IStreamProvider. Ottiene lo stream"
type: docs
url: /it/net/aspose.cells/istreamprovider/initstream/
---
## IStreamProvider.InitStream method

Ottiene lo stream.

```csharp
public void InitStream(StreamProviderOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | StreamProviderOptions |  |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un'istanza della classe demo che implementa IStreamProvider
            var streamProvider = new IStreamProviderMethodInitStreamWithStreamProviderOptionsDemo();
            
            // Prepara StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "custom_path",
                Stream = new MemoryStream()
            };

            try
            {
                // Chiama il metodo InitStream con il parametro StreamProviderOptions
                streamProvider.InitStream(options);
                
                Console.WriteLine("InitStream method executed successfully with StreamProviderOptions parameter");
                
                // Dimostra l'effetto - in questo caso stiamo solo mostrando che lo stream è stato inizializzato
                Console.WriteLine($"Stream initialized: {options.Stream != null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InitStream method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("MethodInitStreamWithStreamProviderOptionsDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Implementazione di InitStream
            Console.WriteLine($"Initializing stream with ResourceLoadingType: {options.ResourceLoadingType}");
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Implementazione di CloseStream
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }
    }
}
```

### Vedi anche

* class [StreamProviderOptions](../../streamprovideroptions/)
* interface [IStreamProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


