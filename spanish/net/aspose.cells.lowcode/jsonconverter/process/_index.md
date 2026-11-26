---
title: "JsonConverter.Process"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método JsonConverter. Convierte el archivo de plantilla dado entre json y otros formatos"
type: docs
url: /es/net/aspose.cells.lowcode/jsonconverter/process/
---
## Process(string, string) {#process_1}

Convierte el archivo de plantilla dado entre json y otros formatos.

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

    public class JsonConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Crea datos JSON de muestra y escribe en un archivo temporal
            string jsonData = "{\"employees\":[{\"name\":\"John\", \"department\":\"Sales\"}, {\"name\":\"Jane\", \"department\":\"Marketing\"}]}";
            string templatePath = "template.json";
            File.WriteAllText(templatePath, jsonData);

            string resultPath = "output.xlsx";

            try
            {
                // Procesa archivos directamente usando el método estático de JsonConverter
                JsonConverter.Process(templatePath, resultPath);

                Console.WriteLine($"Successfully converted JSON to spreadsheet. Output: {resultPath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Conversion error: {ex.Message}");
            }
            finally
            {
                // Limpia el archivo JSON temporal
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### Ver también

* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Convierte entre datos json y otros formatos de archivo de hoja de cálculo.

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
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class JsonConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Crear datos JSON de muestra
            string jsonData = "{\"name\":\"John\", \"age\":30, \"city\":\"New York\"}";
            
            // Crea un flujo de memoria con los datos JSON
            using (MemoryStream stream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(jsonData)))
            {
                // Procesa los datos JSON con opciones LowCode
                JsonConverter.Process(
                    new LowCodeLoadOptions() { InputStream = stream },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.json"
                    });
            }

            Console.WriteLine("JSON processing completed successfully.");
        }
    }
}
```

### Ver también

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


