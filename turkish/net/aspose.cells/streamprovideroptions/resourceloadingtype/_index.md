---
title: "StreamProviderOptions.ResourceLoadingType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StreamProviderOptions özelliği. Yükleme kaynağının türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/streamprovideroptions/resourceloadingtype/
---
## StreamProviderOptions.ResourceLoadingType property

Yükleme kaynağının tipini alır ve ayarlar.

```csharp
public ResourceLoadingType ResourceLoadingType { get; set; }
```

### Örnekler

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
            // Akış sağlayıcı seçenekleriyle çalışma kitabı oluştur
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.UserProvided
            };

            // Farklı kaynak yükleme davranışlarını göster
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Özel bir bellek akışı sağla
                options.Stream = new MemoryStream();
                Console.WriteLine("Using user-provided memory stream");
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Null akışı kullanarak yüklemeyi atla
                options.Stream = Stream.Null;
                Console.WriteLine("Skipping resource loading");
            }
            else
            {
                // Varsayılan dosya yükleme davranışı
                string defaultPath = "default_resource.txt";
                options.Stream = new FileStream(defaultPath, FileMode.Open, FileAccess.Read);
                Console.WriteLine("Loading resource from default path");
            }

            // Temizleme
            options.Stream?.Dispose();
        }
    }
}
```

### Ayrıca Bakınız

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


