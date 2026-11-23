---
title: "BuiltInDocumentPropertyCollection.RevisionNumber"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Obtient ou définit le numéro de révision du document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/revisionnumber/
---
## BuiltInDocumentPropertyCollection.RevisionNumber property

Obtient ou définit le numéro de révision du document.

```csharp
public string RevisionNumber { get; set; }
```

### Remarques

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyRevisionNumberDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définissez la propriété RevisionNumber
            workbook.BuiltInDocumentProperties.RevisionNumber = "1";
            
            // Affichez le RevisionNumber
            Console.WriteLine("Revision Number: " + workbook.BuiltInDocumentProperties.RevisionNumber);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


