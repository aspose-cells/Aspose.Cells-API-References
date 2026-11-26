---
title: "StreamProviderOptions.Stream"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StreamProviderOptions. Obtiene/Establece el flujo"
type: docs
url: /es/net/aspose.cells/streamprovideroptions/stream/
---
## StreamProviderOptions.Stream property

Obtiene/Establece el flujo

```csharp
public Stream Stream { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyStreamDemo
    {
        public static void Run()
        {
            // Crear instancia de StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Caso 1: Cuando no se establece una ruta predeterminada - usar MemoryStream
            options.Stream = new MemoryStream();
            Console.WriteLine("Using MemoryStream: " + (options.Stream is MemoryStream));

            // Caso 2: Simular una ruta predeterminada - usar FileStream
            string outputDir = "output/";
            string defaultPath = "testfile.txt"; // Store path separately since DefaultPath is read-only
            string path = outputDir + Path.GetFileName(defaultPath);
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
            Console.WriteLine("Using FileStream: " + (options.Stream is FileStream));
            
            // Limpiar
            options.Stream.Dispose();
            if (File.Exists(path))
            {
                File.Delete(path);
            }
        }
    }
}
```

### Ver también

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


