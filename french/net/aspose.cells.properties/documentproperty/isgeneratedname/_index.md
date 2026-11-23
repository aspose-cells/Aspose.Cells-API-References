---
title: "DocumentProperty.IsGeneratedName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DocumentProperty. Retourne true si cette propriété n’a pas de nom dans le stockage OLE2 et qu’un nom unique a été généré uniquement pour l’API publique"
type: docs
url: /fr/net/aspose.cells.properties/documentproperty/isgeneratedname/
---
## DocumentProperty.IsGeneratedName property

Renvoie true si cette propriété n'a pas de nom dans le stockage OLE2 et qu'un nom unique a été généré uniquement pour l'API publique.

```csharp
public bool IsGeneratedName { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyPropertyIsGeneratedNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux propriétés de document intégrées
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;
            
            // Accédez aux propriétés de document personnalisées pour les ajouter
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Ajoutez une propriété personnalisée
            DocumentProperty customProperty = customProperties.Add("CustomProperty", "Test Value");
            
            // Affichez IsGeneratedName pour la propriété intégrée
            DocumentProperty authorProperty = properties["Author"];
            Console.WriteLine("Author property IsGeneratedName: " + authorProperty.IsGeneratedName);
            
            // Affichez IsGeneratedName pour la propriété personnalisée
            Console.WriteLine("Custom property IsGeneratedName: " + customProperty.IsGeneratedName);

            // Créez un scénario où une propriété pourrait avoir un nom généré
            // (Remarque : En pratique, IsGeneratedName est en lecture seule et est défini en interne par Aspose.Cells)
            DocumentProperty generatedNameProperty = properties["_PID_GUID"];
            if (generatedNameProperty != null)
            {
                Console.WriteLine("Generated name property IsGeneratedName: " + generatedNameProperty.IsGeneratedName);
            }

            // Enregistrez le classeur
            workbook.Save("PropertyIsGeneratedNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


