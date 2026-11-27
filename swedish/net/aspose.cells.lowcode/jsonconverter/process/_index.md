---
title: "JsonConverter.Process"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonConverter metod. Konverterar given mallfil mellan json och andra format"
type: docs
url: /sv/net/aspose.cells.lowcode/jsonconverter/process/
---
## Process(string, string) {#process_1}

Konverterar given mallfil mellan JSON och andra format.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| templateFile | String | Mallfilen som ska konverteras |
| resultFile | String | Den resulterande filen |

### Exempel

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
            // Skapa exempel‑JSON‑data och skriv till en temporär fil
            string jsonData = "{\"employees\":[{\"name\":\"John\", \"department\":\"Sales\"}, {\"name\":\"Jane\", \"department\":\"Marketing\"}]}";
            string templatePath = "template.json";
            File.WriteAllText(templatePath, jsonData);

            string resultPath = "output.xlsx";

            try
            {
                // Bearbeta filer direkt med JsonConverter:s statiska metod
                JsonConverter.Process(templatePath, resultPath);

                Console.WriteLine($"Successfully converted JSON to spreadsheet. Output: {resultPath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Conversion error: {ex.Message}");
            }
            finally
            {
                // Rensa upp temporär JSON‑fil
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### Se även

* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Konverterar mellan JSON‑data och andra kalkylbladsfilformat.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Alternativ för indata och laddning. |
| saveOptions | LowCodeSaveOptions | Alternativ för utdata och sparning. |

### Exempel

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
            // Skapa exempel‑JSON‑data
            string jsonData = "{\"name\":\"John\", \"age\":30, \"city\":\"New York\"}";
            
            // Skapa ett minnesström med JSON‑data
            using (MemoryStream stream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(jsonData)))
            {
                // Bearbeta JSON‑data med LowCode‑alternativ
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

### Se även

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


