---
title: "StreamProviderOptions.ResourceLoadingType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StreamProviderOptions. Obtiene y establece el tipo de recurso de carga"
type: docs
url: /es/net/aspose.cells/streamprovideroptions/resourceloadingtype/
---
## StreamProviderOptions.ResourceLoadingType property

Obtiene y establece el tipo de recurso de carga.

```csharp
public ResourceLoadingType ResourceLoadingType { get; set; }
```

### Ejemplos

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
            // Crear libro de trabajo con opciones de proveedor de flujo
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.UserProvided
            };

            // Demostrar diferentes comportamientos de carga de recursos
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Proporcionar un flujo de memoria personalizado
                options.Stream = new MemoryStream();
                Console.WriteLine("Using user-provided memory stream");
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Omitir la carga usando un flujo nulo
                options.Stream = Stream.Null;
                Console.WriteLine("Skipping resource loading");
            }
            else
            {
                // Comportamiento predeterminado de carga de archivos
                string defaultPath = "default_resource.txt";
                options.Stream = new FileStream(defaultPath, FileMode.Open, FileAccess.Read);
                Console.WriteLine("Loading resource from default path");
            }

            // Limpieza
            options.Stream?.Dispose();
        }
    }
}
```

### Ver también

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


