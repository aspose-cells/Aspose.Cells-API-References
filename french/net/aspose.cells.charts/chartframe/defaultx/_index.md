---
title: "ChartFrame.DefaultX"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Représente x de la position par défaut en unités de 1/4000 de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/defaultx/
---
## ChartFrame.DefaultX property

Représente x de la position par défaut en unités de 1/4000 de la zone du graphique.

```csharp
[Obsolete("Use ChartFrame.DefaultXRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultX { get; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété ChartFrame.DefaultXRatioToChart à la place. DefaultX = (int)(DefaultXRatioToChart * 4000); Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultXDemo
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
            
            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Accédez au titre du graphique qui hérite de ChartFrame
            chart.Title.Text = "Sample Chart";
            
            // Affichez la position X par défaut du titre du graphique
            Console.WriteLine("Default X position (1/4000 of chart area): " + chart.Title.DefaultX);
            Console.WriteLine("Default X position (ratio of chart area): " + chart.Title.DefaultXRatioToChart);
            
            // Démontrez comment la position par défaut affecte le graphique
            Console.WriteLine("Is default position set? " + chart.Title.IsDefaultPosBeSet);
            
            // Modifiez la position du titre en utilisant les propriétés de ratio (puisque DefaultX est en lecture seule)
            chart.Title.XRatioToChart = 0.2;
            chart.Title.YRatioToChart = 0.05;
            
            // Enregistrez le classeur
            workbook.Save("ChartFrameDefaultXDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


