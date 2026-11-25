---
title: "CellsHelper.IsCloudPlatform"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsHelper. Si prega di impostare questa proprietà su True quando si esegue su una piattaforma cloud come Azure, AWSLambda, ecc."
type: docs
url: /it/net/aspose.cells/cellshelper/iscloudplatform/
---
## CellsHelper.IsCloudPlatform property

Imposta questa proprietà su True quando si esegue su una piattaforma cloud, come: Azure, AWSLambda, ecc.

```csharp
public static bool IsCloudPlatform { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyIsCloudPlatformDemo
    {
        public static void Run()
        {
            // Imposta la proprietà IsCloudPlatform
            CellsHelper.IsCloudPlatform = true;

            // Dimostra l'uso della proprietà
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Mostra come influisce su altre operazioni (esempio)
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

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


