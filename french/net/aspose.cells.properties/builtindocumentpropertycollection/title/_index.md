---
title: "BuiltInDocumentPropertyCollection.Title"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Obtient ou définit le titre du document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/title/
---
## BuiltInDocumentPropertyCollection.Title property

Obtient ou définit le titre du document.

```csharp
public string Title { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTitleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir la propriété Title
            workbook.BuiltInDocumentProperties.Title = "Sample Document Title";
            
            // Afficher la propriété Title
            Console.WriteLine("Document Title: " + workbook.BuiltInDocumentProperties.Title);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


