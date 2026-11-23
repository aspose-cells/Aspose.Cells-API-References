---
title: "ContentTypeProperty.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ContentTypeProperty. Obtient et définit le type de la propriété"
type: docs
url: /fr/net/aspose.cells.properties/contenttypeproperty/type/
---
## ContentTypeProperty.Type property

Obtient et définit le type de la propriété.

```csharp
public string Type { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Ajouter des propriétés de type de contenu avec différents types
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            workbook.ContentTypeProperties.Add("Version", "1.0", "number");
            workbook.ContentTypeProperties.Add("Enabled", "true", "boolean");

            // Accéder et afficher les types de propriétés
            foreach (ContentTypeProperty property in workbook.ContentTypeProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

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


