---
title: "Clase JsonConverter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.JsonConverter. Convertidor para la conversión entre la estructura de datos json y otros formatos de archivo de hoja de cálculo"
type: docs
url: /es/net/aspose.cells.lowcode/jsonconverter/
---
## JsonConverter class

Convertidor para la conversión entre estructuras de datos json y otros formatos de archivo de hoja de cálculo.

```csharp
public class JsonConverter
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Convierte entre datos json y otros formatos de archivo de hoja de cálculo. |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process_1)(string, string) | Convierte el archivo de plantilla dado entre json y otros formatos. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassJsonConverterDemo
    {
        public static void Run()
        {
            string jsonFilePath = "data.json";
            string excelFilePath = "res.xlsx";

            try
            {
                // Convertir JSON a Excel usando Aspose.Cells.LowCode.JsonConverter
                JsonConverter.Process(jsonFilePath, excelFilePath);

                Console.WriteLine("Conversion completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


