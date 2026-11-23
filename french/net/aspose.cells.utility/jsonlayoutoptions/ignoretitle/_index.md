---
title: "JsonLayoutOptions.IgnoreTitle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonLayoutOptions. Ignore les titres des attributs"
type: docs
url: /fr/net/aspose.cells.utility/jsonlayoutoptions/ignoretitle/
---
## JsonLayoutOptions.IgnoreTitle property

Ignore les titres des attributs

```csharp
public bool IgnoreTitle { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyIgnoreTitleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exemple de données JSON
            string jsonInput = @"{
                ""Products"": [
                    {
                        ""Name"": ""Product1"",
                        ""Price"": 100,
                        ""Date"": ""2023-01-15""
                    },
                    {
                        ""Name"": ""Product2"",
                        ""Price"": 200,
                        ""Date"": ""2023-02-20""
                    }
                ]
            }";

            // Définir JsonLayoutOptions avec IgnoreTitle = true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.IgnoreTitle = true;  // This will skip the title row in output
            options.ArrayAsTable = true;
            options.DateFormat = "yyyy/MM/dd";

            // Importer des données JSON
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);

            // Enregistrez le classeur
            workbook.Save("output_ignore_title.xlsx");
        }
    }
}
```

### Voir aussi

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


