---
title: "ContentTypeProperty.IsNillable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ContentTypeProperty. Indique si la valeur peut être vide"
type: docs
url: /fr/net/aspose.cells.properties/contenttypeproperty/isnillable/
---
## ContentTypeProperty.IsNillable property

Indique si la valeur peut être vide.

```csharp
public bool IsNillable { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyIsNillableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Ajouter une propriété de type de contenu
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Accéder à la propriété et définir IsNillable
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.IsNillable = true;
            
            // Vérifier et afficher la valeur IsNillable
            Console.WriteLine($"Property 'Admin' IsNillable: {property.IsNillable}");
            
            workbook.Save("ContentTypePropertyIsNillableDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


