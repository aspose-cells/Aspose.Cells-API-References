---
title: "PlotArea.Height"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PlotArea. Obtient ou définit la hauteur de la boîte englobante du plotarea en unités de 1/4000 de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/plotarea/height/
---
## PlotArea.Height property

Obtient ou définit la hauteur de la boîte englobante du plot-area en unités de 1/4000 de la zone du graphique.

```csharp
[Obsolete("Use PlotArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### Remarques

Le cadre englobant de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Le **X**, **Y**, **Width** et **Height** de **PlotArea** représente la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

Remarque : lorsque Height est définie, la propriété IsInnerMode sera automatiquement définie sur false.

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.HeightRatioToChart à la place. Height = HeightRatioToChart * 4000. Cette propriété sera supprimée 12 mois plus tard, à compter de février 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyHeightDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique
            chart.Calculate();

            // Démontrer la propriété Height
            Console.WriteLine("Chart Area Height: " + chart.ChartArea.Height);
            Console.WriteLine("Plot Area Height: " + chart.PlotArea.Height);

            // Modifier la hauteur de PlotArea
            chart.PlotArea.Height = 2500;
            Console.WriteLine("Modified Plot Area Height: " + chart.PlotArea.Height);
        }
    }
}
```

### Voir aussi

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


