---
title: "JsonLayoutOptions.IgnoreObjectTitle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonLayoutOptions. Indique s'il faut ignorer le titre si l'objet est une propriété d'un autre objet"
type: docs
url: /fr/net/aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/
---
## JsonLayoutOptions.IgnoreObjectTitle property

Indique s'il faut ignorer le titre si l'objet est une propriété d'un autre objet.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreObjectTitle { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété JsonLayoutOptions.IgnoreTitle. Cette propriété sera supprimée 6 mois plus tard, depuis février 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class JsonLayoutOptionsPropertyIgnoreObjectTitleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exemple de données JSON avec des titres d'objet
            string json = @"{
                ""Employees"": {
                    ""Employee"": [
                        { ""Name"": ""John"", ""Age"": 30 },
                        { ""Name"": ""Jane"", ""Age"": 25 }
                    ]
                }
            }";

            // Créer JsonLayoutOptions
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Afficher la valeur actuelle de IgnoreObjectTitle
            Console.WriteLine("Current IgnoreObjectTitle value: " + options.IgnoreObjectTitle);

            // Définir pour ignorer les titres d'objet
            options.IgnoreObjectTitle = true;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // Importer JSON avec IgnoreObjectTitle = true
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Enregistrer avec les titres ignorés
            workbook.Save("IgnoreObjectTitle_True.xlsx");

            // Réinitialiser la feuille de calcul
            worksheet.Cells.Clear();

            // Définir pour inclure les titres d'objet
            options.IgnoreObjectTitle = false;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // Importer JSON avec IgnoreObjectTitle = false
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Enregistrer avec les titres inclus
            workbook.Save("IgnoreObjectTitle_False.xlsx");
        }
    }
}
```

### Voir aussi

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


