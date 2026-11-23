---
title: "JsonLoadOptions.KeptSchema"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonLoadOptions. Indique si le schéma de ce JSON est conservé"
type: docs
url: /fr/net/aspose.cells/jsonloadoptions/keptschema/
---
## JsonLoadOptions.KeptSchema property

Indique s'il faut conserver le schéma de ce JSON.

```csharp
public bool KeptSchema { get; set; }
```

### Remarques

Parfois, nous enregistrons le fichier en JSON après avoir chargé le fichier JSON.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonLoadOptionsPropertyKeptSchemaDemo
    {
        public static void Run()
        {
            // Créer des options de chargement JSON
            JsonLoadOptions options = new JsonLoadOptions();

            // Afficher la valeur par défaut de la propriété KeptSchema
            Console.WriteLine("Default KeptSchema value: " + options.KeptSchema);

            // Définir KeptSchema sur true
            options.KeptSchema = true;
            Console.WriteLine("KeptSchema set to: " + options.KeptSchema);

            // Créer un fichier JSON d'exemple
            string jsonData = @"{
                ""Employees"": [
                    { ""ID"": 1, ""Name"": ""John"", ""Department"": ""Sales"" },
                    { ""ID"": 2, ""Name"": ""Jane"", ""Department"": ""Marketing"" }
                ]
            }";

            System.IO.File.WriteAllText("sample.json", jsonData);

            try
            {
                // Charger JSON avec KeptSchema activé
                Workbook workbook = new Workbook("sample.json", options);

                // Afficher les informations sur le classeur chargé
                Console.WriteLine("Workbook loaded with KeptSchema: " + options.KeptSchema);
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);

                // Enregistrez le classeur
                workbook.Save("KeptSchemaOutput.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


