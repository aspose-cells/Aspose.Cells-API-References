---
title: "CustomProperty.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "CustomProperty propriété. Retourne ou définit le nom de l'objet"
type: docs
url: /fr/net/aspose.cells.properties/customproperty/name/
---
## CustomProperty.Name property

Renvoie ou définit le nom de l'objet.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter une propriété personnalisée avec un nom et une valeur
                worksheet.CustomProperties.Add("SampleName", "SampleValue");

                // Récupérer la propriété personnalisée
                CustomProperty customProperty = worksheet.CustomProperties["SampleName"];

                // Afficher la valeur actuelle de la propriété Name (opération de lecture)
                Console.WriteLine("Custom Property Name: " + customProperty.Name);

                // Définir une nouvelle valeur pour la propriété Name
                customProperty.Name = "UpdatedName";
                Console.WriteLine("Updated Custom Property Name: " + customProperty.Name);

                // Enregistrez le classeur
                workbook.Save("NameDemo.xlsx");
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

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


