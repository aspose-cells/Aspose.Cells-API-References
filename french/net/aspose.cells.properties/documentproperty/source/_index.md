---
title: "DocumentProperty.Source"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DocumentProperty. La source du contenu lié"
type: docs
url: /fr/net/aspose.cells.properties/documentproperty/source/
---
## DocumentProperty.Source property

La source de contenu liée.

```csharp
public string Source { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertySourceDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux propriétés de document personnalisées
            var properties = workbook.Worksheets.CustomDocumentProperties;

            // Ajouter des propriétés
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 1);
            
            // Obtenir les propriétés et afficher leurs sources
            Console.WriteLine("Property Sources:");
            Console.WriteLine($"Author: {properties["Author"].Source}");
            Console.WriteLine($"CreatedDate: {properties["CreatedDate"].Source}");
            Console.WriteLine($"Revision: {properties["Revision"].Source}");

            // Enregistrez le classeur
            workbook.Save("DocumentPropertiesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


