---
title: "JsonSaveOptions.Schemas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonSaveOptions. Le schéma json original de chaque feuille de calcul"
type: docs
url: /fr/net/aspose.cells/jsonsaveoptions/schemas/
---
## JsonSaveOptions.Schemas property

Le schéma JSON original de chaque feuille de calcul.

```csharp
public string[] Schemas { get; set; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Données JSON d'exemple à importer
            string jsonData = @"{
                ""Products"": [
                    {
                        ""ID"": 101,
                        ""Name"": ""Product A"",
                        ""Price"": 99.99
                    }
                ]
            }";

            // Importer les données JSON dans la feuille de calcul
            JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, new JsonLayoutOptions());

            // Schéma d'exemple pour la validation
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

            // Configurer les options d'enregistrement JSON avec le schéma
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.Schemas = new string[] { schema };
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // Enregistrer le classeur avec les options JSON
            string outputPath = "output_with_schema.json";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("Workbook saved with JSON schema validation.");
        }
    }
}
```

### Voir aussi

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


