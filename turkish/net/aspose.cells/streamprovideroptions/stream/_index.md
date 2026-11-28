---
title: "StreamProviderOptions.Stream"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StreamProviderOptions özelliği. Akışı alır/ayarlar"
type: docs
url: /tr/net/aspose.cells/streamprovideroptions/stream/
---
## StreamProviderOptions.Stream property

Akışı alır/ayarlar.

```csharp
public Stream Stream { get; set; }
```

### Örnekler

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
            // StreamProviderOptions örneği oluştur
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Durum 1: Varsayılan yol ayarlanmamışsa - MemoryStream kullan
            options.Stream = new MemoryStream();
            Console.WriteLine("Using MemoryStream: " + (options.Stream is MemoryStream));

            // Durum 2: Varsayılan yol olduğu simüle et - FileStream kullan
            string outputDir = "output/";
            string defaultPath = "testfile.txt"; // Store path separately since DefaultPath is read-only
            string path = outputDir + Path.GetFileName(defaultPath);
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
            Console.WriteLine("Using FileStream: " + (options.Stream is FileStream));
            
            // Temizle
            options.Stream.Dispose();
            if (File.Exists(path))
            {
                File.Delete(path);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


