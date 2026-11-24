---
title: "StreamProviderOptions.DefaultPath"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StreamProviderOptions-Eigenschaft. Der standardmäßige Pfad‑URL, der in der erzeugten HTML‑Datei für die referenzierte Quelle gespeichert wird. Zum Beispiel werden die Blattdaten in xxx_files/sheet001.htm gespeichert; die im Haupt‑HTML‑File verwendete URL sollte etwa srcxxx_files/sheet001.htm lauten."
type: docs
url: /de/net/aspose.cells/streamprovideroptions/defaultpath/
---
## StreamProviderOptions.DefaultPath property

Der Standardpfad (URL), der in der erzeugten html-Datei für die referenzierte Quelle gespeichert wird. Zum Beispiel werden die Blattdaten in xxx_files/sheet001.htm gespeichert, die in der Haupt‑html‑Datei verwendete URL sollte etwa \"src=\"xxx_files/sheet001.htm\"\" sein.

```csharp
public string DefaultPath { get; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyDefaultPathDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();
            
            // Erstelle StreamProviderOptions mit ResourceLoadingType und DefaultPath
            StreamProviderOptions options = new StreamProviderOptions(ResourceLoadingType.Default, "1.DefaultPathExample");
            
            // Demonstration der Verwendung von DefaultPath
            Console.WriteLine("StreamProviderOptions DefaultPath: " + options.DefaultPath);
            
            // Beispiel für die Verwendung der Optionen mit einem Stream (vereinfachte Demonstration)
            using (MemoryStream stream = new MemoryStream())
            {
                options.Stream = stream;
                
                if (options.DefaultPath.IndexOf("1.") >= 0)
                {
                    Console.WriteLine("Processing stream for path: " + options.DefaultPath);
                    // Operationen mit dem Stream ausführen
                    workbook.Save(stream, SaveFormat.Xlsx);
                }
            }
        }
    }
}
```

### Siehe auch

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


