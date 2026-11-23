---
title: "JsonLayoutOptions.JsonLayoutOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur JsonLayoutOptions. Constructeur de chargement des options de mise en page JSON"
type: docs
url: /fr/net/aspose.cells.utility/jsonlayoutoptions/jsonlayoutoptions/
---
## JsonLayoutOptions constructor

Constructeur de chargement des options de mise en page JSON.

```csharp
public JsonLayoutOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créer des données JSON d'exemple
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": {
                    ""Street"": ""123 Main St"",
                    ""City"": ""New York""
                }
            }";

            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Initialiser JsonLayoutOptions en utilisant le constructeur
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Définir les options
            options.ArrayAsTable = true;
            options.IgnoreArrayTitle = false;
            options.IgnoreObjectTitle = false;

            // Importez les données JSON dans la feuille de calcul
            JsonUtility.ImportData(json, workbook.Worksheets[0].Cells, 0, 0, options);

            // Enregistrez le classeur
            workbook.Save("JsonImportDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


