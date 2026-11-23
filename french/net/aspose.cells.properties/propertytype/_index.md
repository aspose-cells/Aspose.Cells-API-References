---
title: "Énumération PropertyType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Properties.PropertyType. Spécifie le type de données d'une propriété de document"
type: docs
url: /fr/net/aspose.cells.properties/propertytype/
---
## PropertyType enumeration

Spécifie le type de données d'une propriété de document.

```csharp
public enum PropertyType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Boolean | `0` | La propriété est une valeur booléenne. |
| DateTime | `1` | La propriété est une valeur de date et heure. |
| Double | `2` | La propriété est un nombre à virgule flottante. |
| Number | `3` | La propriété est un nombre entier. |
| String | `4` | La propriété est une valeur chaîne. |
| Blob | `5` | La propriété est un tableau d'octets. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class PropertyTypeDemo
    {
        public static void PropertyTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux propriétés de document intégrées
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Définir certaines propriétés intégrées
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Subject = "Demonstration of PropertyType";
            builtInProperties.Company = "Aspose";

            // Accéder aux propriétés de document personnalisées
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Ajouter des propriétés personnalisées de différents types
            customProperties.Add("IsReviewed", true); // Boolean
            customProperties.Add("ReviewDate", DateTime.Now); // DateTime
            customProperties.Add("Rating", 4.5); // Double
            customProperties.Add("Pages", 100); // Number
            customProperties.Add("Summary", "This is a sample workbook for demonstrating PropertyType."); // String

            // Récupérer et afficher les propriétés personnalisées
            foreach (DocumentProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // Enregistrez le classeur
            workbook.Save("PropertyTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


