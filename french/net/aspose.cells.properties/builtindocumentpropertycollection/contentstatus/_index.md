---
title: "BuiltInDocumentPropertyCollection.ContentStatus"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Obtient ou définit le statut du contenu du document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/contentstatus/
---
## BuiltInDocumentPropertyCollection.ContentStatus property

Obtient ou définit le statut du contenu du document.

```csharp
public string ContentStatus { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentStatusDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Définir les propriétés de document intégrées incluant ContentStatus
            workbook.BuiltInDocumentProperties.ContentStatus = "Draft";
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";

            // Enregistrez le classeur
            workbook.Save("DocumentWithContentStatus.xlsx", SaveFormat.Xlsx);

            // Chargez le classeur enregistré pour vérifier les propriétés
            Workbook loadedWorkbook = new Workbook("DocumentWithContentStatus.xlsx");
            
            // Afficher la propriété ContentStatus
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


