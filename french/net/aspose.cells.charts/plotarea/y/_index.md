---
title: "PlotArea.Y"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PlotArea. Obtient ou définit la coordonnée y du coin supérieur du cadre englobant de la zone de tracé en unités de 1/4000 de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/plotarea/y/
---
## PlotArea.Y property

Obtient ou définit la coordonnée y du coin supérieur du cadre englobant de la zone de tracé en unités de 1/4000 de la zone du graphique.

```csharp
[Obsolete("Use PlotArea.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Remarques

Le cadre englobant de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Le **X**, **Y**, **Width** et **Height** de **PlotArea** représente la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

Remarque : lorsque Y est défini, la propriété IsInnerMode sera automatiquement définie sur false.

NOTE : ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.YRatioToChart à la place. Y = YRatioToChart * 4000. Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Données d'exemple
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(50);

            // Créer un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Définir les données du graphique
            chart.NSeries.Add("B1:B2", false);
            chart.NSeries.CategoryData = "A1:A2";

            // Configurer la zone de tracé
            chart.PlotArea.Width = 300;
            chart.PlotArea.Height = 200;
            chart.PlotArea.X = 100;
            chart.PlotArea.Y = 150; // Demonstrating Y property usage

            // Enregistrez le classeur
            workbook.Save("PlotAreaPropertyYDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


