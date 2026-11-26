---
title: "ConversionUtility.Convert"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ConversionUtility. Convierte archivos Excel a otros formatos"
type: docs
url: /es/net/aspose.cells.utility/conversionutility/convert/
---
## Convert(string, string) {#convert_1}

Convierte archivos Excel a otros formatos.

```csharp
public static void Convert(string source, string saveAs)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | String | El nombre del archivo fuente. |
| saveAs | String | El nombre del archivo esperado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ConversionUtilityMethodConvertWithStringStringDemo
    {
        public static void Run()
        {
            // Inicializar rutas de archivo de origen y destino
            string sourcePath = "source.xlsx";
            string destPath = "output.pdf";
            // Convertir archivo Excel a PDF
            ConversionUtility.Convert(sourcePath, destPath);

            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### Ver también

* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## Convert(string, LoadOptions, string, SaveOptions) {#convert}

Convierte archivos Excel a otros formatos.

```csharp
public static void Convert(string source, LoadOptions loadOptions, string saveAs, 
    SaveOptions saveOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | String | El nombre del archivo fuente. |
| loadOptions | LoadOptions | Las opciones de carga del archivo fuente. |
| saveAs | String | El nombre del archivo esperado. |
| saveOptions | SaveOptions | Las opciones de guardado del archivo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ConversionUtilityMethodConvertWithStringLoadOptionsStringSaveOptDemo
    {
        public static void Run()
        {
            // Rutas de archivo de origen y destino
            string sourceFile = "input.csv";
            string outputFile = "output.xlsx";

            // Crear archivo CSV de ejemplo para demostración
            System.IO.File.WriteAllText(sourceFile, "Name,Age\nJohn,30\nAlice,25");

            try
            {
                // Crear opciones de carga para el archivo CSV
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                
                // Crear opciones de guardado para el archivo XLSX
                SaveOptions saveOptions = new OoxmlSaveOptions();

                // Convertir CSV a XLSX con opciones especificadas
                ConversionUtility.Convert(sourceFile, loadOptions, outputFile, saveOptions);

                Console.WriteLine($"File converted successfully from {sourceFile} to {outputFile}");
                
                // Verificar la conversión cargando el archivo de salida
                Workbook workbook = new Workbook(outputFile);
                Console.WriteLine($"Output file contains {workbook.Worksheets.Count} worksheet(s)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Limpia los archivos temporales
                if (System.IO.File.Exists(sourceFile))
                {
                    System.IO.File.Delete(sourceFile);
                }
            }
        }
    }
}
```

### Ver también

* class [LoadOptions](../../../aspose.cells/loadoptions/)
* class [SaveOptions](../../../aspose.cells/saveoptions/)
* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


