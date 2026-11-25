---
title: "StreamProviderOptions.Stream"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StreamProviderOptions. Ottiene/Imposta lo stream"
type: docs
url: /it/net/aspose.cells/streamprovideroptions/stream/
---
## StreamProviderOptions.Stream property

Ottiene/Imposta lo stream

```csharp
public Stream Stream { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyStreamDemo
    {
        public static void Run()
        {
            // Crea un'istanza di StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Caso 1: Quando non è impostato alcun percorso predefinito - usa MemoryStream
            options.Stream = new MemoryStream();
            Console.WriteLine("Using MemoryStream: " + (options.Stream is MemoryStream));

            // Caso 2: Simula la presenza di un percorso predefinito - usa FileStream
            string outputDir = "output/";
            string defaultPath = "testfile.txt"; // Store path separately since DefaultPath is read-only
            string path = outputDir + Path.GetFileName(defaultPath);
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
            Console.WriteLine("Using FileStream: " + (options.Stream is FileStream));
            
            // Pulisci
            options.Stream.Dispose();
            if (File.Exists(path))
            {
                File.Delete(path);
            }
        }
    }
}
```

### Vedi anche

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


