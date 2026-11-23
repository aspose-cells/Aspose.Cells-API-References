---
title: "DataLabels.ShowPercentage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataLabels. Représente le comportement d'affichage de la valeur de pourcentage d'étiquette de données d'un graphique spécifié. True affiche la valeur du pourcentage. False pour masquer"
type: docs
url: /fr/net/aspose.cells.charts/datalabels/showpercentage/
---
## DataLabels.ShowPercentage property

Représente le comportement d'affichage de la valeur en pourcentage de l'étiquette de données d'un graphique spécifié. Vrai affiche la valeur en pourcentage. Faux masque.

```csharp
public bool ShowPercentage { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowPercentageDemo
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

            // Ajouter un graphique en secteurs
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Activer les étiquettes de données et afficher le pourcentage
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowPercentage = true;
            dataLabels.ShowValue = false;

            // Enregistrez le classeur
            workbook.Save("DataLabelsShowPercentageDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


