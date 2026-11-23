---
title: "JsonLayoutOptions.KeptSchema"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonLayoutOptions. Indique s'il faut conserver le schéma de ce json"
type: docs
url: /fr/net/aspose.cells.utility/jsonlayoutoptions/keptschema/
---
## JsonLayoutOptions.KeptSchema property

Indique s'il faut conserver le schéma de ce JSON.

```csharp
public bool KeptSchema { get; set; }
```

### Remarques

Parfois, nous enregistrons le fichier en JSON après avoir chargé le fichier JSON.

### Exemples

```csharp
using System;
using System.IO;
using System.Text.Json;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyKeptSchemaDemo
    {
        public class Data
        {
            public string RootProperty { get; set; }
            public Payload Payload { get; set; }
        }

        public class Payload
        {
            public ArrayData[] Array { get; set; }
            public string PayloadProperty { get; set; }
            public PayloadStruct PayloadStruct { get; set; }
        }

        public class ArrayData
        {
            public string ArrayProperty { get; set; }
        }

        public struct PayloadStruct
        {
            public string PayloadProperty1 { get; set; }
            public string PayloadProperty2 { get; set; }
        }

        public static void Run()
        {
            // Créer des données d'exemple
            var data = new Data()
            {
                RootProperty = "RootValue",
                Payload = new Payload()
                {
                    Array = new[]
                    {
                        new ArrayData() { ArrayProperty = "item1" },
                        new ArrayData() { ArrayProperty = "item2" }
                    },
                    PayloadProperty = "PayloadValue",
                    PayloadStruct = new PayloadStruct()
                    {
                        PayloadProperty1 = "struct1",
                        PayloadProperty2 = "struct2"
                    }
                }
            };

            // Sérialiser en JSON en utilisant System.Text.Json
            string json = JsonSerializer.Serialize(new[] { data });

            // Créer un classeur et importer JSON
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.KeptSchema = true; // Demonstrate KeptSchema usage
            
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, layoutOptions);

            // Enregistrer et afficher les résultats
            string outputPath = "output/";
            Directory.CreateDirectory(outputPath);
            
            workbook.Save(outputPath + "KeptSchemaDemo.xlsx", SaveFormat.Xlsx);
            workbook.Save(outputPath + "KeptSchemaDemo.json", new JsonSaveOptions()
            {
                ExportNestedStructure = true
            });

            Console.WriteLine("Files saved successfully. Check output directory.");
        }
    }
}
```

### Voir aussi

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


