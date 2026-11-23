---
title: "BuiltInDocumentPropertyCollection.CreatedUniversalTime"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Obtient ou définit l'heure universelle de la création du document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/createduniversaltime/
---
## BuiltInDocumentPropertyCollection.CreatedUniversalTime property

Obtient ou définit l'heure universelle de création du document.

```csharp
public DateTime CreatedUniversalTime { get; set; }
```

### Remarques

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCreatedUniversalTimeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir la propriété CreatedUniversalTime
            DateTime creationTime = new DateTime(2023, 5, 15, 15, 30, 0, DateTimeKind.Utc);
            workbook.BuiltInDocumentProperties.CreatedUniversalTime = creationTime;
            
            // Afficher la propriété CreatedUniversalTime
            Console.WriteLine("Document created (UTC): " + 
                workbook.BuiltInDocumentProperties.CreatedUniversalTime.ToString());
            
            // Enregistrez le classeur
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


