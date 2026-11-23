---
title: "Classe CustomProperty"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Properties.CustomProperty class. Représente une propriété personnalisée qui stocke des paires nom‑valeur de données utilisateur arbitraires pour la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.properties/customproperty/
---
## CustomProperty class

Représente une propriété personnalisée qui stocke des paires nom‑valeur de données arbitraires définies par l'utilisateur pour la feuille de calcul.

```csharp
public class CustomProperty
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BinaryValue](../../aspose.cells.properties/customproperty/binaryvalue/) { get; set; } | Obtient et définit la valeur binaire de la propriété personnalisée. |
| [Name](../../aspose.cells.properties/customproperty/name/) { get; set; } | Renvoie ou définit le nom de l'objet. |
| [StringValue](../../aspose.cells.properties/customproperty/stringvalue/) { get; set; } | (**Obsolete.**) Retourne ou définit la valeur de la propriété personnalisée. |
| [Value](../../aspose.cells.properties/customproperty/value/) { get; set; } | Renvoie ou définit la valeur de la propriété personnalisée. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyDemo
    {
        public static void CustomPropertyExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Accéder à la collection CustomProperties
            CustomPropertyCollection customProperties = sheet.CustomProperties;

            // Ajouter des propriétés personnalisées
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("LastModified", DateTime.Now.ToString());

            // Accéder et afficher les propriétés personnalisées
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Enregistrez le classeur
            workbook.Save("CustomPropertyExample.xlsx");
            workbook.Save("CustomPropertyExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


