---
title: "JsonLayoutOptions.NumberFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonLayoutOptions. Obtient et définit le format de la valeur numérique"
type: docs
url: /fr/net/aspose.cells.utility/jsonlayoutoptions/numberformat/
---
## JsonLayoutOptions.NumberFormat property

Obtient et définit le format de la valeur numérique.

```csharp
public string NumberFormat { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Créer une chaîne de données JSON
            string jsonData = @"{
                ""Products"": [
                    { ""ID"": 101, ""Price"": 19.95, ""Date"": ""2023-05-15"" },
                    { ""ID"": 102, ""Price"": 29.99, ""Date"": ""2023-06-20"" }
                ]
            }";

            // Créer JsonLayoutOptions avec NumberFormat
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                NumberFormat = "0.00",
                DateFormat = "yyyy-MM-dd"
            };

            // Créer un classeur à partir de JSON
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(jsonData);
            JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, layoutOptions);

            // Enregistrer sous Excel
            workbook.Save("JsonNumberFormatDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


