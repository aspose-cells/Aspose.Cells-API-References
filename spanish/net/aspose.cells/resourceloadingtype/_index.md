---
title: "Enumeración ResourceLoadingType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.ResourceLoadingType. Representa cómo cargar el recurso vinculado"
type: docs
url: /es/net/aspose.cells/resourceloadingtype/
---
## ResourceLoadingType enumeration

Representa cómo cargar el recurso vinculado.

```csharp
public enum ResourceLoadingType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Default | `0` | Carga este recurso como de costumbre. |
| Skip | `1` | Omite la carga de este recurso. |
| UserProvided | `2` | Utiliza el flujo proporcionado por el usuario |

### Ejemplos

```csharp
using Aspose.Cells;
using System;
using System.IO;

namespace AsposeCellsExamples
{
    public class ResourceLoadingTypeDemo
    {
        public static void ResourceLoadingTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Resource");
            worksheet.Cells["A2"].PutValue("Default");
            worksheet.Cells["A3"].PutValue("Skip");
            worksheet.Cells["A4"].PutValue("UserProvided");

            // Guarda el libro de trabajo en HTML con un proveedor de flujo personalizado
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                StreamProvider = new CustomStreamProvider()
            };

            workbook.Save("ResourceLoadingTypeExample.html", saveOptions);
        }
    }

    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Proporciona un flujo personalizado para el recurso
                options.Stream = new MemoryStream();
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Omitir la carga del recurso
                options.Stream = Stream.Null;
            }
            else
            {
                // Cargar el recurso como de costumbre
                options.Stream = new FileStream(options.DefaultPath, FileMode.Open, FileAccess.Read);
            }
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Cierra el flujo si no es nulo
            options.Stream?.Close();
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


