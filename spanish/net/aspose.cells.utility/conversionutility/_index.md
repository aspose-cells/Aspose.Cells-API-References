---
title: "Clase ConversionUtility"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Utility.ConversionUtility. Representa una utilidad para convertir archivos a otros formatos"
type: docs
url: /es/net/aspose.cells.utility/conversionutility/
---
## ConversionUtility class

Representa una utilidad para convertir archivos a otros formatos.

```csharp
public class ConversionUtility
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert_1)(string, string) | Convierte archivos Excel a otros formatos. |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert)(string, LoadOptions, string, SaveOptions) | Convierte archivos Excel a otros formatos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;
    using System.IO;

    public class UtilityClassConversionUtilityDemo
    {
        public static void Run()
        {
            // Crea un archivo CSV de ejemplo para la conversión
            string sourceFile = "sample.csv";
            string outputFile = "converted.xlsx";

            try
            {
                // Crea contenido CSV de ejemplo
                File.WriteAllText(sourceFile, "Product,Price,Quantity\nApple,1.50,100\nBanana,0.75,150\nOrange,1.25,120");

                // Convierte CSV a XLSX usando el método estático de conversión
                ConversionUtility.Convert(sourceFile, outputFile);

                Console.WriteLine($"Successfully converted {sourceFile} to {outputFile}");

                // Verifica la conversión comprobando si el archivo de salida existe
                if (File.Exists(outputFile))
                {
                    Console.WriteLine("Output file created successfully");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Limpia los archivos temporales
                if (File.Exists(sourceFile))
                {
                    File.Delete(sourceFile);
                }
                if (File.Exists(outputFile))
                {
                    File.Delete(outputFile);
                }
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


