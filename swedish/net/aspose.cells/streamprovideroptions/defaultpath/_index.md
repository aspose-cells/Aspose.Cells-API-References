---
title: "StreamProviderOptions.DefaultPath"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StreamProviderOptions‑egenskap. Standard‑pathURL sparad i den genererade html‑filen för den refererade källan. Till exempel sparas bladdata i xxx_files/sheet001.htm; URL:en som används i huvud‑html‑filen bör vara som srcxxx_files/sheet001.htm"
type: docs
url: /sv/net/aspose.cells/streamprovideroptions/defaultpath/
---
## StreamProviderOptions.DefaultPath property

Den standard sökvägen (URL) som sparas i den genererade html‑filen för den refererade källan. Till exempel, bladdata sparad i xxx_files/sheet001.htm, URL:en som används i huvud‑html‑filen bör vara som "src=\"xxx_files/sheet001.htm\""

```csharp
public string DefaultPath { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa StreamProviderOptions med ResourceLoadingType och DefaultPath
            StreamProviderOptions options = new StreamProviderOptions(ResourceLoadingType.Default, "1.DefaultPathExample");
            
            // Demonstrera användning av DefaultPath
            Console.WriteLine("StreamProviderOptions DefaultPath: " + options.DefaultPath);
            
            // Exempel på att använda alternativen med en ström (förenklad demonstration)
            using (MemoryStream stream = new MemoryStream())
            {
                options.Stream = stream;
                
                if (options.DefaultPath.IndexOf("1.") >= 0)
                {
                    Console.WriteLine("Processing stream for path: " + options.DefaultPath);
                    // Utför operationer med strömmen
                    workbook.Save(stream, SaveFormat.Xlsx);
                }
            }
        }
    }
}
```

### Se även

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


