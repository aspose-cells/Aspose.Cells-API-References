---
title: "BuiltInDocumentPropertyCollection.Characters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Représente une estimation du nombre de caractères dans le document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/characters/
---
## BuiltInDocumentPropertyCollection.Characters property

Représente une estimation du nombre de caractères dans le document.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Characters { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyCharactersDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux propriétés de document intégrées
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Afficher la valeur actuelle de Characters (propriété obsolète)
            Console.WriteLine("Current Characters value: " + properties.Characters);

            // Définir une nouvelle valeur pour Characters (propriété obsolète)
            properties.Characters = 1500;
            Console.WriteLine("Updated Characters value: " + properties.Characters);

            // Ajouter du contenu pour démontrer l'effet de la propriété
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
            
            // Enregistrez le classeur
            workbook.Save("PropertyCharactersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


