---
title: "CellsHelper.IsCloudPlatform"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper‑egenskap. Ställ in denna egenskap till True när du kör på en molnplattform som Azure, AWSLambda etc."
type: docs
url: /sv/net/aspose.cells/cellshelper/iscloudplatform/
---
## CellsHelper.IsCloudPlatform property

Ställ in denna egenskap till True när du kör på en molnplattform, såsom: Azure, AWSLambda, etc.

```csharp
public static bool IsCloudPlatform { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyIsCloudPlatformDemo
    {
        public static void Run()
        {
            // Ange egenskapen IsCloudPlatform
            CellsHelper.IsCloudPlatform = true;

            // Demonstrera egenskapens användning
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Visa hur det påverkar andra operationer (exempel)
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

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


