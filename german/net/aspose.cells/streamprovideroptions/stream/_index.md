---
title: "StreamProviderOptions.Stream"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StreamProviderOptions property. Liest/Setzt den Stream"
type: docs
url: /de/net/aspose.cells/streamprovideroptions/stream/
---
## StreamProviderOptions.Stream property

Liest/Setzt den Stream

```csharp
public Stream Stream { get; set; }
```

### Beispiele

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
            // Erstellen Sie eine Instanz von StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Fall 1: Wenn kein Standardpfad festgelegt ist – MemoryStream verwenden
            options.Stream = new MemoryStream();
            Console.WriteLine("Using MemoryStream: " + (options.Stream is MemoryStream));

            // Fall 2: Simulieren Sie einen vorhandenen Standardpfad – FileStream verwenden
            string outputDir = "output/";
            string defaultPath = "testfile.txt"; // Store path separately since DefaultPath is read-only
            string path = outputDir + Path.GetFileName(defaultPath);
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
            Console.WriteLine("Using FileStream: " + (options.Stream is FileStream));
            
            // Aufräumen
            options.Stream.Dispose();
            if (File.Exists(path))
            {
                File.Delete(path);
            }
        }
    }
}
```

### Siehe auch

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


