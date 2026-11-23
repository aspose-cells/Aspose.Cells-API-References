---
title: "RevisionLogCollection.HighlightChanges"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode RevisionLogCollection. Met en évidence les modifications du classeur partagé"
type: docs
url: /fr/net/aspose.cells.revisions/revisionlogcollection/highlightchanges/
---
## RevisionLogCollection.HighlightChanges method

Met en évidence les modifications du classeur partagé.

```csharp
public void HighlightChanges(HighlightChangesOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | HighlightChangesOptions | Définir les options de filtrage des modifications à suivre. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionMethodHighlightChangesWithHighlightChangesOptionsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple et des révisions
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Mettre en évidence les modifications avec des options
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            workbook.Worksheets.RevisionLogs.HighlightChanges(options);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HighlightChangesOptions](../../highlightchangesoptions/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


