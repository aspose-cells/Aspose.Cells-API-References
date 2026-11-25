---
title: "JsonSaveOptions.Schemas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonSaveOptions. Lo schema json originale di ogni foglio di lavoro"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/schemas/
---
## JsonSaveOptions.Schemas property

Lo schema JSON originale di ogni foglio di lavoro.

```csharp
public string[] Schemas { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Dati JSON di esempio da importare
            string jsonData = @"{
                ""Products"": [
                    {
                        ""ID"": 101,
                        ""Name"": ""Product A"",
                        ""Price"": 99.99
                    }
                ]
            }";

            // Importa dati JSON nel foglio di lavoro
            JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, new JsonLayoutOptions());

            // Schema di esempio per la convalida
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

            // Configura le opzioni di salvataggio JSON con schema
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.Schemas = new string[] { schema };
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // Salva la cartella di lavoro con le opzioni JSON
            string outputPath = "output_with_schema.json";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("Workbook saved with JSON schema validation.");
        }
    }
}
```

### Vedi anche

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


