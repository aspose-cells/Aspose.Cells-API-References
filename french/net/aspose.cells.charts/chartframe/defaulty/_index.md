---
title: "ChartFrame.DefaultY"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Représente le y de la position par défaut en unités de 1/4000 de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/defaulty/
---
## ChartFrame.DefaultY property

Représente le y de la position par défaut en unités de 1/4000 de la zone du graphique.

```csharp
[Obsolete("Use ChartFrame.DefaultYRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultY { get; }
```

### Remarques

NOTE : Cet élément est maintenant obsolète. Veuillez utiliser la propriété ChartFrame.DefaultYRatioToChart à la place. DefaultY = (int)(DefaultYRatioToChart * 4000); Cette propriété sera supprimée 12 mois plus tard, à compter de février 2025. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultYDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Accédez au titre du graphique qui hérite de ChartFrame
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;
            
            // Afficher la valeur actuelle de DefaultY (propriété en lecture seule)
            Console.WriteLine("DefaultY value (1/4000 of chart area): " + chartFrame.DefaultY);
            Console.WriteLine("DefaultY ratio to chart area: " + chartFrame.DefaultYRatioToChart);
            
            // Démontrer comment DefaultY affecte le positionnement en le comparant à la position actuelle
            Console.WriteLine("Current Y position (ratio): " + chartFrame.YRatioToChart);
            
            // Réinitialiser la position à la valeur par défaut en utilisant SetPositionAuto()
            chartFrame.SetPositionAuto();
            Console.WriteLine("Y position after reset (ratio): " + chartFrame.YRatioToChart);
            
            // Enregistrer le résultat
            workbook.Save("ChartFramePropertyDefaultYDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


