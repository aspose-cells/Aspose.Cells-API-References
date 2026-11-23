---
title: "CellsHelper.IsCloudPlatform"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsHelper. Veuillez définir cette propriété sur True lorsque vous exécutez sur une plateforme cloud telle qu'Azure, AWSLambda, etc."
type: docs
url: /fr/net/aspose.cells/cellshelper/iscloudplatform/
---
## CellsHelper.IsCloudPlatform property

Veuillez définir cette propriété sur True lors de l'exécution sur une plateforme cloud, telle que : Azure, AWSLambda, etc,

```csharp
public static bool IsCloudPlatform { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyIsCloudPlatformDemo
    {
        public static void Run()
        {
            // Définissez la propriété IsCloudPlatform
            CellsHelper.IsCloudPlatform = true;

            // Démontrez l'utilisation de la propriété
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Montrez comment cela affecte d'autres opérations (exemple)
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

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


