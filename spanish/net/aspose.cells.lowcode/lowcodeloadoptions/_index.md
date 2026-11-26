---
title: "Clase LowCodeLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.LowCodeLoadOptions. Opciones para cargar el archivo de plantilla"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodeloadoptions/
---
## LowCodeLoadOptions class

Opciones para cargar el archivo de plantilla.

```csharp
public class LowCodeLoadOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LowCodeLoadOptions](lowcodeloadoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [InputFile](../../aspose.cells.lowcode/lowcodeloadoptions/inputfile/) { get; set; } | Obtiene y establece el archivo (con ruta si es necesario) de la plantilla. |
| [InputStream](../../aspose.cells.lowcode/lowcodeloadoptions/inputstream/) { get; set; } | Obtiene y establece el Stream de la plantilla. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            // Crea un Stream de ejemplo (en memoria para propósitos de demostración)
            using (MemoryStream stream = new MemoryStream())
            {
                // Crea un nuevo libro de trabajo y guárdalo en un stream para la demostración
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Save(stream, SaveFormat.Xlsx);

                // Restablece la posición del stream
                stream.Position = 0;

                // Crea y usa LowCodeLoadOptions
                var loadOptions = new LowCodeLoadOptions()
                {
                    InputStream = stream
                };

                // Ejemplo de uso - normalmente se pasaría a un método de procesamiento
                Console.WriteLine($"Loading with LowCode options from stream of length: {loadOptions.InputStream.Length}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


