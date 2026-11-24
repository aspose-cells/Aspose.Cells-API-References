---
title: "CellsHelper.IsCloudPlatform"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper property. Bitte setzen Sie diese Eigenschaft auf True, wenn Sie auf einer Cloud-Plattform wie Azure, AWSLambda usw. ausführen."
type: docs
url: /de/net/aspose.cells/cellshelper/iscloudplatform/
---
## CellsHelper.IsCloudPlatform property

Bitte setzen Sie diese Eigenschaft auf True, wenn Sie auf einer Cloud-Plattform laufen, z. B.: Azure, AWSLambda, etc,

```csharp
public static bool IsCloudPlatform { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyIsCloudPlatformDemo
    {
        public static void Run()
        {
            // Setzen Sie die IsCloudPlatform-Eigenschaft
            CellsHelper.IsCloudPlatform = true;

            // Demonstrieren Sie die Verwendung der Eigenschaft
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Zeigen Sie, wie es andere Vorgänge beeinflusst (Beispiel)
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

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


