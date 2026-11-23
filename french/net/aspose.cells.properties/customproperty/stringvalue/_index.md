---
title: "CustomProperty.StringValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "CustomProperty propriété. Retourne ou définit la valeur de la propriété personnalisée"
type: docs
url: /fr/net/aspose.cells.properties/customproperty/stringvalue/
---
## CustomProperty.StringValue property

Renvoie ou définit la valeur de la propriété personnalisée.

```csharp
[Obsolete("Use CustomProperty.Value property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValue { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété CustomProperty.Value. Cette propriété sera supprimée 12 mois plus tard depuis juin 2010. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyStringValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter une propriété personnalisée avec une valeur de chaîne
                worksheet.CustomProperties.Add("SampleProperty", "Test Value");

                // Récupérer la propriété personnalisée
                CustomProperty customProperty = worksheet.CustomProperties["SampleProperty"];

                // Afficher la propriété StringValue (opération de lecture)
                Console.WriteLine("StringValue: " + customProperty.StringValue);

                // Définir une nouvelle valeur pour la propriété StringValue
                customProperty.StringValue = "Updated Value";
                Console.WriteLine("Updated StringValue: " + customProperty.StringValue);

                // Enregistrez le classeur
                workbook.Save("StringValueDemo.xlsx");
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


