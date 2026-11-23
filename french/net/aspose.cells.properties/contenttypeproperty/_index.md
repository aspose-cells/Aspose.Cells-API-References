---
title: "Classe ContentTypeProperty"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Properties.ContentTypeProperty. Représente les informations d'identifiant"
type: docs
url: /fr/net/aspose.cells.properties/contenttypeproperty/
---
## ContentTypeProperty class

Représente les informations d'identifiant.

```csharp
public class ContentTypeProperty
```

## Propriétés

| Nom | Description |
| --- | --- |
| [IsNillable](../../aspose.cells.properties/contenttypeproperty/isnillable/) { get; set; } | Indique si la valeur peut être vide. |
| [Name](../../aspose.cells.properties/contenttypeproperty/name/) { get; set; } | Renvoie ou définit le nom de l'objet. |
| [Type](../../aspose.cells.properties/contenttypeproperty/type/) { get; set; } | Obtient et définit le type de la propriété. |
| [Value](../../aspose.cells.properties/contenttypeproperty/value/) { get; set; } | Renvoie ou définit la valeur de la propriété de type de contenu. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class ContentTypePropertyDemo
    {
        public static void ContentTypePropertyExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle propriété de type de contenu
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // Accéder à la propriété nouvellement ajoutée
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Définition des propriétés
            property.Name = "Admin";
            property.Value = "Aspose";
            property.Type = "text";
            property.IsNillable = true;

            // Enregistrez le fichier Excel
            workbook.Save("ContentTypePropertyExample.xlsx");
            workbook.Save("ContentTypePropertyExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


