---
title: "StreamProviderOptions.ResourceLoadingType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StreamProviderOptions-egenskap. Hämtar och sätter typen av resurshämtning"
type: docs
url: /sv/net/aspose.cells/streamprovideroptions/resourceloadingtype/
---
## StreamProviderOptions.ResourceLoadingType property

Hämtar och anger typen av laddningsresurs.

```csharp
public ResourceLoadingType ResourceLoadingType { get; set; }
```

### Exempel

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
            // Skapa arbetsbok med alternativ för strömleverantör
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.UserProvided
            };

            // Demonstrera olika resursladdningsbeteenden
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Tillhandahåll en anpassad minnesström
                options.Stream = new MemoryStream();
                Console.WriteLine("Using user-provided memory stream");
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Hoppa över laddning genom att använda nullström
                options.Stream = Stream.Null;
                Console.WriteLine("Skipping resource loading");
            }
            else
            {
                // Standardbeteende för filladdning
                string defaultPath = "default_resource.txt";
                options.Stream = new FileStream(defaultPath, FileMode.Open, FileAccess.Read);
                Console.WriteLine("Loading resource from default path");
            }

            // Städa upp
            options.Stream?.Dispose();
        }
    }
}
```

### Se även

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


