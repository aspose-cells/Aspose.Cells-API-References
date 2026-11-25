---
title: "StreamProviderOptions.ResourceLoadingType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StreamProviderOptions. Ottiene e imposta il tipo di risorsa da caricare"
type: docs
url: /it/net/aspose.cells/streamprovideroptions/resourceloadingtype/
---
## StreamProviderOptions.ResourceLoadingType property

Ottiene e imposta il tipo di risorsa di caricamento.

```csharp
public ResourceLoadingType ResourceLoadingType { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyResourceLoadingTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con le opzioni del provider di stream
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.UserProvided
            };

            // Dimostra diversi comportamenti di caricamento delle risorse
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Fornisci un memory stream personalizzato
                options.Stream = new MemoryStream();
                Console.WriteLine("Using user-provided memory stream");
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Salta il caricamento usando uno stream nullo
                options.Stream = Stream.Null;
                Console.WriteLine("Skipping resource loading");
            }
            else
            {
                // Comportamento predefinito di caricamento dei file
                string defaultPath = "default_resource.txt";
                options.Stream = new FileStream(defaultPath, FileMode.Open, FileAccess.Read);
                Console.WriteLine("Loading resource from default path");
            }

            // Pulizia
            options.Stream?.Dispose();
        }
    }
}
```

### Vedi anche

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


