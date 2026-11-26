---
title: "CellsHelper.IsCloudPlatform"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellsHelper. Por favor, establezca esta propiedad en True cuando se ejecute en una plataforma en la nube como Azure, AWSLambda, etc."
type: docs
url: /es/net/aspose.cells/cellshelper/iscloudplatform/
---
## CellsHelper.IsCloudPlatform property

Por favor, establezca esta propiedad en True al ejecutar en una plataforma en la nube, como: Azure, AWSLambda, etc,

```csharp
public static bool IsCloudPlatform { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyIsCloudPlatformDemo
    {
        public static void Run()
        {
            // Establecer la propiedad IsCloudPlatform
            CellsHelper.IsCloudPlatform = true;

            // Demostrar el uso de la propiedad
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Mostrar cómo afecta a otras operaciones (ejemplo)
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

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


