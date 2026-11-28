---
title: "CellsHelper.IsCloudPlatform"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper özelliği. Azure, AWSLambda vb. bir bulut platformunda çalışırken bu özelliği True olarak ayarlayın"
type: docs
url: /tr/net/aspose.cells/cellshelper/iscloudplatform/
---
## CellsHelper.IsCloudPlatform property

Bulut platformunda (Azure, AWSLambda vb.) çalışırken lütfen bu özelliği True olarak ayarlayın,

```csharp
public static bool IsCloudPlatform { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyIsCloudPlatformDemo
    {
        public static void Run()
        {
            // IsCloudPlatform özelliğini ayarla
            CellsHelper.IsCloudPlatform = true;

            // Özelliğin kullanımını göster
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Diğer işlemleri nasıl etkilediğini göster (örnek)
            if (CellsHelper.IsCloudPlatform)
            {
                Console.WriteLine("Running in cloud environment - using cloud-specific settings");
                CellsHelper.StartupPath = "/cloud_storage/aspose/cells";
            }
            else
            {
                Console.WriteLine("Running in local environment");
                CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


