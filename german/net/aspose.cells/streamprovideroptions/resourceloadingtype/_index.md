---
title: "StreamProviderOptions.ResourceLoadingType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StreamProviderOptions property. Gibt und setzt den Typ der zu ladenden Ressource"
type: docs
url: /de/net/aspose.cells/streamprovideroptions/resourceloadingtype/
---
## StreamProviderOptions.ResourceLoadingType property

Liest und setzt den Typ der zu ladenden Ressource.

```csharp
public ResourceLoadingType ResourceLoadingType { get; set; }
```

### Beispiele

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
            // Erstellen Sie ein Arbeitsbuch mit StreamProviderOptions
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.UserProvided
            };

            // Demonstrieren Sie verschiedene Verhaltensweisen beim Laden von Ressourcen
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Stellen Sie einen benutzerdefinierten MemoryStream bereit
                options.Stream = new MemoryStream();
                Console.WriteLine("Using user-provided memory stream");
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Laden überspringen, indem ein Null-Stream verwendet wird
                options.Stream = Stream.Null;
                Console.WriteLine("Skipping resource loading");
            }
            else
            {
                // Standardverhalten beim Laden von Dateien
                string defaultPath = "default_resource.txt";
                options.Stream = new FileStream(defaultPath, FileMode.Open, FileAccess.Read);
                Console.WriteLine("Loading resource from default path");
            }

            // Aufräumen
            options.Stream?.Dispose();
        }
    }
}
```

### Siehe auch

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


