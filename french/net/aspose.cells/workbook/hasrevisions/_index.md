---
title: "Workbook.HasRevisions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Indique si le classeur possède des modifications suivies"
type: docs
url: /fr/net/aspose.cells/workbook/hasrevisions/
---
## Workbook.HasRevisions property

Obtient si le classeur possède des modifications suivies

```csharp
public bool HasRevisions { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasRevisionsDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des révisions
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Effectuez une modification qui créera une révision
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Vérifier si le classeur possède des révisions
            Console.WriteLine("Workbook has revisions: " + workbook.HasRevisions);
            
            // Accepter toutes les révisions (le cas échéant)
            if (workbook.HasRevisions)
            {
                workbook.AcceptAllRevisions();
            }
            
            // Vérifiez à nouveau après avoir accepté les révisions
            Console.WriteLine("Workbook has revisions after accepting: " + workbook.HasRevisions);
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


