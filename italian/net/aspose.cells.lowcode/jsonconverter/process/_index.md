---
title: "JsonConverter.Process"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo JsonConverter. Converte il file modello fornito tra json e altri formati"
type: docs
url: /it/net/aspose.cells.lowcode/jsonconverter/process/
---
## Process(string, string) {#process_1}

Converte il file modello fornito tra json e altri formati.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| templateFile | String | Il file modello da convertire |
| resultFile | String | Il file risultante |

### Esempi

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
            // Crea dati JSON di esempio e scrivili in un file temporaneo
            string jsonData = "{\"employees\":[{\"name\":\"John\", \"department\":\"Sales\"}, {\"name\":\"Jane\", \"department\":\"Marketing\"}]}";
            string templatePath = "template.json";
            File.WriteAllText(templatePath, jsonData);

            string resultPath = "output.xlsx";

            try
            {
                // Elabora i file direttamente usando il metodo statico di JsonConverter
                JsonConverter.Process(templatePath, resultPath);

                Console.WriteLine($"Successfully converted JSON to spreadsheet. Output: {resultPath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Conversion error: {ex.Message}");
            }
            finally
            {
                // Pulisci il file JSON temporaneo
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### Vedi anche

* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Converte tra dati json e altri formati di foglio di calcolo.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opzioni per l'input e il caricamento |
| saveOptions | LowCodeSaveOptions | Opzioni per l'output e il salvataggio |

### Esempi

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
            // Crea dati JSON di esempio
            string jsonData = "{\"name\":\"John\", \"age\":30, \"city\":\"New York\"}";
            
            // Crea uno stream di memoria con i dati JSON
            using (MemoryStream stream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(jsonData)))
            {
                // Elabora i dati JSON con le opzioni LowCode
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

### Vedi anche

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


