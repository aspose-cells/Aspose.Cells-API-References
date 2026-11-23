---
title: "ChartFrame.IsDefaultPosBeSet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Indique si la position par défaut DefaultX DefaultY DefaultWidth et DefaultHeight est définie"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/isdefaultposbeset/
---
## ChartFrame.IsDefaultPosBeSet property

Indique si la position par défaut (DefaultX, DefaultY, DefaultWidth et DefaultHeight) est définie.

```csharp
public bool IsDefaultPosBeSet { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsDefaultPosBeSetDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Bar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder aux étiquettes de données
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Démontrer la propriété IsDefaultPosBeSet
            Console.WriteLine("IsDefaultPosBeSet before setting position: " + dataLabels.IsDefaultPosBeSet);
            
            // Modifier la position et vérifier à nouveau la propriété
            dataLabels.Position = LabelPositionType.InsideBase;
            Console.WriteLine("IsDefaultPosBeSet after setting position: " + dataLabels.IsDefaultPosBeSet);
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


