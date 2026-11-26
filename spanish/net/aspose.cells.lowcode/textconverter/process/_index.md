---
title: "TextConverter.Process"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método TextConverter. Convierte el archivo de plantilla dado entre archivos basados en texto y otros formatos"
type: docs
url: /es/net/aspose.cells.lowcode/textconverter/process/
---
## Process(string, string) {#process_1}

Convierte el archivo de plantilla dado entre archivos basados en texto y otros formatos.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| templateFile | String | El archivo de plantilla a convertir |
| resultFile | String | El archivo resultante |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class TextConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            string inputFile = "input.csv";
            string outputFile = "output.xlsx";

            // Crea un archivo CSV de ejemplo
            File.WriteAllText(inputFile, $"Column1,Column2{Environment.NewLine}Data1,Data2{Environment.NewLine}Data3,Data4");

            try
            {
                // Llama al método estático Process directamente sin instanciar TextConverter
                TextConverter.Process(inputFile, outputFile);
                
                Console.WriteLine($"Process method successfully converted {inputFile} to {outputFile}");
                Console.WriteLine($"Converted file exists: {File.Exists(outputFile)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
            finally
            {
                // Limpiar archivos temporales
                if (File.Exists(inputFile))
                {
                    File.Delete(inputFile);
                }
            }
        }
    }
}
```

### Ver también

* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Convierte el formato de archivo entre formatos basados en texto y otros formatos de archivo de hoja de cálculo

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opciones de entrada y carga |
| saveOptions | LowCodeSaveOptions | Opciones de salida y guardado |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class TextConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Crea un archivo de texto de ejemplo
            string inputText = "Sample text content";
            string inputPath = "input.txt";
            File.WriteAllText(inputPath, inputText);

            // Procesa el archivo de texto con opciones LowCode
            using (FileStream inputStream = new FileStream(inputPath, FileMode.Open))
            {
                TextConverter.Process(
                    new LowCodeLoadOptions() { InputStream = inputStream },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.txt"
                    }
                );
            }

            Console.WriteLine("Text processing completed successfully.");
        }
    }
}
```

### Ver también

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


