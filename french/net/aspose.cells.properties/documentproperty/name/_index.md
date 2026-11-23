---
title: "DocumentProperty.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "DocumentProperty property. Retourne le nom de la propriété"
type: docs
url: /fr/net/aspose.cells.properties/documentproperty/name/
---
## DocumentProperty.Name property

Renvoie le nom de la propriété.

```csharp
public string Name { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder aux propriétés du document
            BuiltInDocumentPropertyCollection builtInProps = workbook.BuiltInDocumentProperties;
            CustomDocumentPropertyCollection customProps = workbook.CustomDocumentProperties;
            
            // Ajouter une propriété personnalisée et démontrer l'utilisation de Name
            DocumentProperty authorProperty = customProps.Add("Author", "John Doe");
            Console.WriteLine("Property Name: " + authorProperty.Name);
            Console.WriteLine("Property Value: " + authorProperty.Value);
            
            // Accéder à une propriété intégrée par son nom
            DocumentProperty titleProperty = builtInProps["Title"];
            titleProperty.Value = "Sample Document";
            Console.WriteLine("Title Property Name: " + titleProperty.Name);
            Console.WriteLine("Title Property Value: " + titleProperty.Value);
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


