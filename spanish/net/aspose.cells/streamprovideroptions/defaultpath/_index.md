---
title: "StreamProviderOptions.DefaultPath"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StreamProviderOptions. La URL de ruta predeterminada guardada en el archivo HTML generado para la fuente referenciada. Por ejemplo, los datos de la hoja guardados en xxx_files/sheet001.htm, la URL utilizada en el archivo HTML principal debería ser como srcxxx_files/sheet001.htm"
type: docs
url: /es/net/aspose.cells/streamprovideroptions/defaultpath/
---
## StreamProviderOptions.DefaultPath property

La ruta predeterminada (URL) guardada en el archivo html generado para la fuente referenciada. Por ejemplo, los datos de la hoja guardados en xxx_files/sheet001.htm, la url utilizada en el archivo html principal debería ser como "src=\"xxx_files/sheet001.htm\""

```csharp
public string DefaultPath { get; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyDefaultPathDemo
    {
        public static void Run()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();
            
            // Crear StreamProviderOptions con ResourceLoadingType y DefaultPath
            StreamProviderOptions options = new StreamProviderOptions(ResourceLoadingType.Default, "1.DefaultPathExample");
            
            // Demostrar el uso de DefaultPath
            Console.WriteLine("StreamProviderOptions DefaultPath: " + options.DefaultPath);
            
            // Ejemplo de uso de las opciones con un flujo (demostración simplificada)
            using (MemoryStream stream = new MemoryStream())
            {
                options.Stream = stream;
                
                if (options.DefaultPath.IndexOf("1.") >= 0)
                {
                    Console.WriteLine("Processing stream for path: " + options.DefaultPath);
                    // Realizar operaciones con el flujo
                    workbook.Save(stream, SaveFormat.Xlsx);
                }
            }
        }
    }
}
```

### Ver también

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


