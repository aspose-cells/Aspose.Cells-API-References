---
title: "DataLabels.ShowValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "DataLabels propriété. Représente le comportement d'affichage des valeurs d'étiquette de données d'un graphique spécifié. True affiche les valeurs. False pour les masquer"
type: docs
url: /fr/net/aspose.cells.charts/datalabels/showvalue/
---
## DataLabels.ShowValue property

Représente le comportement d'affichage des valeurs de l'étiquette de données d'un graphique spécifié. Vrai affiche les valeurs. Faux masque.

```csharp
public bool ShowValue { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowValueDemo
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

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Activez les étiquettes de données et affichez les valeurs
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.Position = LabelPositionType.Center;

            // Enregistrez le classeur
            workbook.Save("DataLabelsShowValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


