---
title: "BuiltInDocumentPropertyCollection.CharactersWithSpaces"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Représente une estimation du nombre de caractères, espaces compris, dans le document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/characterswithspaces/
---
## BuiltInDocumentPropertyCollection.CharactersWithSpaces property

Représente une estimation du nombre de caractères (espaces compris) dans le document.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CharactersWithSpaces { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyCharactersWithSpacesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux propriétés de document intégrées
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Afficher la valeur actuelle de CharactersWithSpaces
            Console.WriteLine("Current CharactersWithSpaces value: " + properties.CharactersWithSpaces);
            
            // Définir une nouvelle valeur pour CharactersWithSpaces
            properties.CharactersWithSpaces = 1500;
            Console.WriteLine("Updated CharactersWithSpaces value: " + properties.CharactersWithSpaces);
            
            // Ajouter du contenu pour démontrer l'effet de la propriété
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
            worksheet.Cells["A2"].PutValue("The CharactersWithSpaces property represents estimated character count including spaces.");
            
            // Enregistrez le classeur
            workbook.Save("PropertyCharactersWithSpacesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


