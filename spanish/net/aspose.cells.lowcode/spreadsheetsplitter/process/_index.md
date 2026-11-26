---
title: "SpreadsheetSplitter.Process"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SpreadsheetSplitter. Divide el archivo de plantilla dado en múltiples partes"
type: docs
url: /es/net/aspose.cells.lowcode/spreadsheetsplitter/process/
---
## Process(string, string) {#process_1}

Divide el archivo de plantilla proporcionado en múltiples partes.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| templateFile | String | El archivo de plantilla a dividir |
| resultFile | String | El archivo resultante (patrón de nombre) |

### Observaciones

Los archivos de salida se crearán a partir del archivo resultante especificado añadiendo el número de secuencia de la hoja y la parte dividida. Por ejemplo, si el archivo de salida especificado es Split.xlsx, los archivos generados serán Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ...

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetSplitterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con múltiples hojas de cálculo
            Workbook templateWorkbook = new Workbook();
            Worksheet sheet1 = templateWorkbook.Worksheets.Add("SalesData");
            sheet1.Cells["A1"].PutValue("Product");
            Worksheet sheet2 = templateWorkbook.Worksheets.Add("Inventory");
            sheet2.Cells["A1"].PutValue("test data");

            // Guardar como archivo de plantilla
            string templatePath = "SplitterTemplate.xlsx";
            templateWorkbook.Save(templatePath, SaveFormat.Xlsx);

            // Definir patrón de salida del resultado
            string resultPattern = "SplitResult_";
            
            try
            {
                // Procesar la plantilla directamente usando el método estático
                SpreadsheetSplitter.Process(templatePath, resultPattern);
                
                Console.WriteLine($"Spreadsheet split successfully using pattern: {resultPattern}");
                Console.WriteLine("Check output directory for split files");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during spreadsheet splitting: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeSplitOptions) {#process}

Divide el archivo de hoja de cálculo en varias partes.

```csharp
public static void Process(LowCodeSplitOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | LowCodeSplitOptions | Opciones para dividir la hoja de cálculo |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetSplitterMethodProcessWithLowCodeSplitOptionsDemo
    {
        public static void Run()
        {

            // Inicializar opciones de división
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions
            {
                LoadOptions = new LowCodeLoadOptions { InputFile = "split.xlsx" },
                SaveOptionsProvider = new CustomLowCodeSaveOptionsProvider()
            };

            try
            {
                // Ejecutar la división de la hoja de cálculo usando un método estático
                SpreadsheetSplitter.Process(splitOptions);
                
                Console.WriteLine($"Spreadsheet split successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Split operation failed: {ex.Message}");
            }
        }
    }

    // Implementación concreta de AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        {
            base.Finish(part);
        }
        // Implementa el método abstracto requerido
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### Ver también

* class [LowCodeSplitOptions](../../lowcodesplitoptions/)
* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


