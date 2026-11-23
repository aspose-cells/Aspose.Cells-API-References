---
title: "BuiltInDocumentPropertyCollection.Paragraphs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Représente une estimation du nombre de paragraphes dans le document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/paragraphs/
---
## BuiltInDocumentPropertyCollection.Paragraphs property

Représente une estimation du nombre de paragraphes dans le document.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Paragraphs { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyParagraphsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux propriétés de document intégrées
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Afficher la valeur actuelle de Paragraphs (propriété obsolète)
            Console.WriteLine("Current Paragraphs value: " + properties.Paragraphs);

            // Définir une nouvelle valeur pour Paragraphs (propriété obsolète)
            properties.Paragraphs = 15;
            Console.WriteLine("Updated Paragraphs value: " + properties.Paragraphs);

            // Ajouter du contenu pour démontrer l'effet de la propriété
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is paragraph 1");
            worksheet.Cells["A2"].PutValue("This is paragraph 2");
            worksheet.Cells["A3"].PutValue("This is paragraph 3");

            // Enregistrez le classeur
            workbook.Save("PropertyParagraphsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


