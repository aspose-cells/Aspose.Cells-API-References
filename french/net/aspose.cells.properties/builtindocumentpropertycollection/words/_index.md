---
title: "BuiltInDocumentPropertyCollection.Words"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "BuiltInDocumentPropertyCollection property. Représente une estimation du nombre de mots dans le document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/words/
---
## BuiltInDocumentPropertyCollection.Words property

Représente une estimation du nombre de mots dans le document.

```csharp
public int Words { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyWordsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux propriétés de document intégrées
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Définir la propriété Words
            builtInProperties.Words = 250;

            // Ajouter du contenu à la feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample document");
            worksheet.Cells["A2"].PutValue("Demonstrating the Words property");
            worksheet.Cells["A3"].PutValue("Total words will be set to 250");

            // Enregistrez le classeur
            workbook.Save("DocumentWithWordsProperty.xlsx");

            Console.WriteLine("Document created with Words property set to: " + builtInProperties.Words);
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


