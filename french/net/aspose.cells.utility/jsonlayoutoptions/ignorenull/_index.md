---
title: "JsonLayoutOptions.IgnoreNull"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonLayoutOptions. Indique si la valeur null est ignorée"
type: docs
url: /fr/net/aspose.cells.utility/jsonlayoutoptions/ignorenull/
---
## JsonLayoutOptions.IgnoreNull property

Indique s'il faut ignorer les valeurs nulles.

```csharp
public bool IgnoreNull { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyIgnoreNullDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Exemple de JSON avec des valeurs null
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": null,
                ""Salary"": 500.00
            }";

            // Configurer les options d'importation JSON avec IgnoreNull défini sur true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.IgnoreNull = true;
            options.NumberFormat = "$0.00";

            // Importez les données JSON dans la feuille de calcul
            JsonUtility.ImportData(json, cells, 0, 0, options);

            // Vérifier les données importées (l'adresse null doit être ignorée)
            Console.WriteLine("Name: " + cells["A2"].StringValue);    // John
            Console.WriteLine("Age: " + cells["B2"].IntValue);        // 30
            Console.WriteLine("Address exists: " + (cells["C2"].Value != null)); // False
            Console.WriteLine("Salary: " + cells["D2"].StringValue);  // $500.00

            // Enregistrez le classeur
            workbook.Save("JsonIgnoreNullDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


