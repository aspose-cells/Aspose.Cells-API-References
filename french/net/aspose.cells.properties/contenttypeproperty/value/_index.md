---
title: "ContentTypeProperty.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ContentTypeProperty. Retourne ou définit la valeur de la propriété de type de contenu"
type: docs
url: /fr/net/aspose.cells.properties/contenttypeproperty/value/
---
## ContentTypeProperty.Value property

Renvoie ou définit la valeur de la propriété de type de contenu.

```csharp
public string Value { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Ajouter une propriété de type de contenu
            workbook.ContentTypeProperties.Add("Admin", "InitialValue", "text");
            
            // Accéder et modifier la valeur de la propriété
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.Value = "Aspose"; // Demonstrating Value property usage
            
            // Enregistrez le classeur
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


