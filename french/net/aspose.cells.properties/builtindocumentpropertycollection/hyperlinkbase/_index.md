---
title: "BuiltInDocumentPropertyCollection.HyperlinkBase"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Obtient ou définit la propriété hyperlinkbase"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/hyperlinkbase/
---
## BuiltInDocumentPropertyCollection.HyperlinkBase property

Obtient ou définit la propriété hyperlinkbase.

```csharp
public string HyperlinkBase { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyHyperlinkBaseDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Définir la propriété HyperlinkBase
            workbook.BuiltInDocumentProperties.HyperlinkBase = "http://www.example.com";

            // Définir une autre propriété à des fins de démonstration
            workbook.BuiltInDocumentProperties.Title = "Sample Workbook";

            // Enregistrez le classeur
            workbook.Save("HyperlinkBaseDemo.xlsx", SaveFormat.Xlsx);

            // Chargez le classeur enregistré pour vérifier les propriétés
            Workbook loadedWorkbook = new Workbook("HyperlinkBaseDemo.xlsx");
            
            // Afficher les propriétés dans la console
            Console.WriteLine("HyperlinkBase: " + loadedWorkbook.BuiltInDocumentProperties.HyperlinkBase);
            Console.WriteLine("Title: " + loadedWorkbook.BuiltInDocumentProperties.Title);
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


