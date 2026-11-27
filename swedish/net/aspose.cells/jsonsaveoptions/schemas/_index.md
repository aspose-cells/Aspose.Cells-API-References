---
title: "JsonSaveOptions.Schemas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-egenskap. Det ursprungliga json-schemat för varje kalkylblad"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/schemas/
---
## JsonSaveOptions.Schemas property

Det ursprungliga json-schemat för varje kalkylblad.

```csharp
public string[] Schemas { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertySchemasDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Exempel på JSON-data att importera
            string jsonData = @"{
                ""Products"": [
                    {
                        ""ID"": 101,
                        ""Name"": ""Product A"",
                        ""Price"": 99.99
                    }
                ]
            }";

            // Importera JSON-data till kalkylbladet
            JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, new JsonLayoutOptions());

            // Exempelschema för validering
            string schema = @"{
                ""$schema"": ""http://json-schema.org/draft-07/schema#"",
                ""type"": ""object"",
                ""properties"": {
                    ""Products"": {
                        ""type"": ""array"",
                        ""items"": {
                            ""type"": ""object"",
                            ""properties"": {
                                ""ID"": { ""type"": ""integer"" },
                                ""Name"": { ""type"": ""string"" },
                                ""Price"": { ""type"": ""number"" }
                            },
                            ""required"": [""ID"", ""Name"", ""Price""]
                        }
                    }
                },
                ""required"": [""Products""]
            }";

            // Konfigurera JSON-sparalternativ med schema
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.Schemas = new string[] { schema };
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // Spara arbetsbok med JSON-alternativ
            string outputPath = "output_with_schema.json";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("Workbook saved with JSON schema validation.");
        }
    }
}
```

### Se även

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


