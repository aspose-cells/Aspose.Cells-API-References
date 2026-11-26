---
title: "Clase StreamProviderOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.StreamProviderOptions. Representa las opciones de flujo"
type: docs
url: /es/net/aspose.cells/streamprovideroptions/
---
## StreamProviderOptions class

Representa las opciones de flujo.

```csharp
public class StreamProviderOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [StreamProviderOptions](streamprovideroptions/#constructor)() | Inicializa una nueva instancia de la clase `StreamProviderOptions`. |
| [StreamProviderOptions](streamprovideroptions/#constructor_1)(ResourceLoadingType, string) | Inicializa una nueva instancia de la clase `StreamProviderOptions`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CustomPath](../../aspose.cells/streamprovideroptions/custompath/) { get; set; } | La ruta personalizada del usuario (URL) guardada en el archivo HTML generado para la fuente referenciada. Si no es definida por el usuario, se utilizará DefaultPath. Por ejemplo, los datos de la hoja serán guardados por el usuario en d:/sheet001.htm, la URL utilizada en el archivo HTML principal debería ser "d:/sheet001.htm" u otra ruta relativa válida que pueda ser accedida por el archivo HTML principal. |
| [DefaultPath](../../aspose.cells/streamprovideroptions/defaultpath/) { get; } | La ruta predeterminada (URL) guardada en el archivo html generado para la fuente referenciada. Por ejemplo, los datos de la hoja guardados en xxx_files/sheet001.htm, la url utilizada en el archivo html principal debería ser como "src=\"xxx_files/sheet001.htm\"" |
| [ResourceLoadingType](../../aspose.cells/streamprovideroptions/resourceloadingtype/) { get; set; } | Obtiene y establece el tipo de recurso de carga. |
| [Stream](../../aspose.cells/streamprovideroptions/stream/) { get; set; } | Obtiene/Establece el flujo |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassStreamProviderOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Establecer un flujo de memoria para la demostración
            options.Stream = new MemoryStream();
            
            // Usar el flujo (ejemplo: guardar el libro de trabajo en el flujo)
            workbook.Save(options.Stream, SaveFormat.Xlsx);
            
            // Demostrar el cierre del flujo
            CloseStream(options);
        }

        public static void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


