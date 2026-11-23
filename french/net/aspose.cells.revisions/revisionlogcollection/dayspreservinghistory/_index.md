---
title: "RevisionLogCollection.DaysPreservingHistory"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionLogCollection. Obtient et définit le nombre de jours pendant lesquels l'application de feuille de calcul conservera l'historique des modifications pour ce classeur"
type: docs
url: /fr/net/aspose.cells.revisions/revisionlogcollection/dayspreservinghistory/
---
## RevisionLogCollection.DaysPreservingHistory property

Obtient et définit le nombre de jours pendant lesquels l'application de feuille de calcul conservera l'historique des modifications pour ce classeur.

```csharp
public int DaysPreservingHistory { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionPropertyDaysPreservingHistoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Value");
            
            // Définir la propriété DaysPreservingHistory
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 40;
            
            string outputPath = "output_DaysPreservingHistory.xlsx";
            workbook.Save(outputPath);
            
            // Recharger pour vérifier la propriété
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("DaysPreservingHistory: " + 
                loadedWorkbook.Worksheets.RevisionLogs.DaysPreservingHistory);
        }
    }
}
```

### Voir aussi

* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


