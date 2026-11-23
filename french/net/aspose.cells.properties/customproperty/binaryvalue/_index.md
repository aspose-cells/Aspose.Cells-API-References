---
title: "CustomProperty.BinaryValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CustomProperty. Obtient et définit la valeur binaire de la propriété personnalisée"
type: docs
url: /fr/net/aspose.cells.properties/customproperty/binaryvalue/
---
## CustomProperty.BinaryValue property

Obtient et définit la valeur binaire de la propriété personnalisée.

```csharp
public byte[] BinaryValue { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyBinaryValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une propriété personnalisée avec une valeur d'exemple
            worksheet.CustomProperties.Add("SampleBinary", "01010101");

            try
            {
                // Récupérer la propriété personnalisée
                CustomProperty prop = worksheet.CustomProperties["SampleBinary"];

                // Afficher le Nom et la Valeur de la propriété personnalisée
                Console.WriteLine($"Custom Property Name : {prop.Name}");
                Console.WriteLine($"Custom Property Value: {prop.Value}");

                // NOTE : La réflexion pour CustomProperty n'inclut pas de propriété BinaryValue.
                // La valeur disponible basée sur une chaîne est accessible via la propriété 'Value'.

                // Enregistrer le classeur (facultatif)
                workbook.Save("BinaryValueDemo.xlsx");
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


