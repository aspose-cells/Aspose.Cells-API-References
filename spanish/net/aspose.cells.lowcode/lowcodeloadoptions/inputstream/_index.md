---
title: "LowCodeLoadOptions.InputStream"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeLoadOptions. Obtiene y establece el Stream de la plantilla"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodeloadoptions/inputstream/
---
## LowCodeLoadOptions.InputStream property

Obtiene y establece el Stream de la plantilla.

```csharp
public Stream InputStream { get; set; }
```

### Observaciones

Al establecer un Stream no nulo en esta propiedad, el valor previamente establecido para [`InputFile`](../inputfile/) será ignorado.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeLoadOptionsPropertyInputStreamDemo
    {
        public static void Run()
        {
            // Crear datos de ejemplo en un Stream de memoria
            byte[] data = { 0x48, 0x65, 0x6C, 0x6C, 0x6F }; // "Hello" in bytes
            using (MemoryStream stream = new MemoryStream(data))
            {
                // Crear opciones de carga con InputStream
                var loadOptions = new LowCodeLoadOptions() { InputStream = stream };

                // Crear un nuevo libro de trabajo usando el stream
                using (Workbook workbook = new Workbook(stream))
                {
                    // Acceder a la primera hoja de cálculo
                    Worksheet worksheet = workbook.Worksheets[0];
                    
                    // Demostrar que el contenido fue cargado
                    Console.WriteLine("First cell value: " + worksheet.Cells["A1"].Value);
                }
            }
        }
    }
}
```

### Ver también

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


