---
title: "ChartTextFrame.IsDeleted"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartTextFrame. Indique si cette étiquette de données est supprimée"
type: docs
url: /fr/net/aspose.cells.charts/charttextframe/isdeleted/
---
## ChartTextFrame.IsDeleted property

Indique si cette étiquette de données est supprimée.

```csharp
public bool IsDeleted { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder aux étiquettes de données et démontrer la propriété IsDeleted
            chart.NSeries[0].DataLabels.ShowValue = true;
            bool isDeletedBefore = chart.NSeries[0].DataLabels.IsDeleted;
            
            // Supprimer les étiquettes de données en définissant ShowValue sur false
            chart.NSeries[0].DataLabels.ShowValue = false;
            bool isDeletedAfter = chart.NSeries[0].DataLabels.IsDeleted;

            Console.WriteLine($"DataLabels IsDeleted before removal: {isDeletedBefore}");
            Console.WriteLine($"DataLabels IsDeleted after removal: {isDeletedAfter}");
        }
    }
}
```

### Voir aussi

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


