---
title: "IStreamProvider.CloseStream"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IStreamProvider. Chiude lo stream"
type: docs
url: /it/net/aspose.cells/istreamprovider/closestream/
---
## IStreamProvider.CloseStream method

Chiude lo stream.

```csharp
public void CloseStream(StreamProviderOptions options)
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

    public class IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo : IStreamProvider
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un'istanza della classe demo che implementa IStreamProvider
            var streamProvider = new IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo();
            
            // Crea StreamProviderOptions
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "output_files/sheet001.htm",
                Stream = new MemoryStream()
            };

            try
            {
                // Chiama il metodo CloseStream
                streamProvider.CloseStream(options);
                
                Console.WriteLine("CloseStream method executed successfully with StreamProviderOptions");
                
                // Dimostra l'effetto - in uno scenario reale, questo chiuderebbe lo stream
                Console.WriteLine($"Stream closed status: {options.Stream == null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CloseStream method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("IStreamProviderCloseStreamDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Implementazione richiesta dall'interfaccia
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

### Vedi anche

* class [StreamProviderOptions](../../streamprovideroptions/)
* interface [IStreamProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


