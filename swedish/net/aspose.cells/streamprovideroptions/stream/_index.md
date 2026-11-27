---
title: "StreamProviderOptions.Stream"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StreamProviderOptions-egenskap. Hämtar/sätter strömmen"
type: docs
url: /sv/net/aspose.cells/streamprovideroptions/stream/
---
## StreamProviderOptions.Stream property

Hämtar/anger strömmen

```csharp
public Stream Stream { get; set; }
```

### Exempel

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
            // Skapa en StreamProviderOptions-instans
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Fall 1: När ingen standard‑sökväg är inställd – använd MemoryStream
            options.Stream = new MemoryStream();
            Console.WriteLine("Using MemoryStream: " + (options.Stream is MemoryStream));

            // Fall 2: Simulera att ha en standard‑sökväg – använd FileStream
            string outputDir = "output/";
            string defaultPath = "testfile.txt"; // Store path separately since DefaultPath is read-only
            string path = outputDir + Path.GetFileName(defaultPath);
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
            Console.WriteLine("Using FileStream: " + (options.Stream is FileStream));
            
            // Rensa upp
            options.Stream.Dispose();
            if (File.Exists(path))
            {
                File.Delete(path);
            }
        }
    }
}
```

### Se även

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


