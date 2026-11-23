---
title: "BuiltInDocumentPropertyCollection.Lines"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Représente une estimation du nombre de lignes dans le document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/lines/
---
## BuiltInDocumentPropertyCollection.Lines property

Représente une estimation du nombre de lignes dans le document.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Lines { get; set; }
```

### Remarques

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyLinesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux propriétés de document intégrées
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Afficher la valeur actuelle de Lines (estimation du nombre de lignes dans le document)
            Console.WriteLine("Current Lines value: " + properties.Lines);
            
            // Définir une nouvelle valeur pour la propriété Lines
            properties.Lines = 150;
            
            // Ajouter du contenu pour démontrer le but de la propriété
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Line " + (i + 1);
            }
            
            // Enregistrez le classeur
            workbook.Save("PropertyLinesDemo.xlsx");
            
            // Remarque : la propriété Lines est une estimation et ne se mettra pas à jour automatiquement avec le contenu réel
            // Elle est principalement utilisée à des fins de métadonnées de document
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


