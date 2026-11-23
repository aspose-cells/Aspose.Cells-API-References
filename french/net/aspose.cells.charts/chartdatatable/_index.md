---
title: "Classe ChartDataTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.ChartDataTable. Représente un tableau de données de graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartdatatable/
---
## ChartDataTable class

Représente un tableau de données du graphique.

```csharp
public class ChartDataTable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/chartdatatable/autoscalefont/) { get; set; } | Vrai si le texte de l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai. |
| [BackgroundMode](../../aspose.cells.charts/chartdatatable/backgroundmode/) { get; set; } | Obtient et définit le mode d'affichage de l'arrière-plan |
| [Border](../../aspose.cells.charts/chartdatatable/border/) { get; } | Renvoie un objet Border qui représente la bordure de l'objet |
| [Font](../../aspose.cells.charts/chartdatatable/font/) { get; } | Obtient un objet [`Font`](./font/) qui représente le paramètre de police du tableau de données de graphique spécifié. |
| [HasBorderHorizontal](../../aspose.cells.charts/chartdatatable/hasborderhorizontal/) { get; set; } | (**Obsolete.**) Vrai si le tableau de données du graphique possède des bordures de cellules horizontales |
| [HasBorderOutline](../../aspose.cells.charts/chartdatatable/hasborderoutline/) { get; set; } | (**Obsolete.**) Vrai si le tableau de données du graphique a des bordures extérieures |
| [HasBorderVertical](../../aspose.cells.charts/chartdatatable/hasbordervertical/) { get; set; } | (**Obsolete.**) Vrai si le tableau de données du graphique a des bordures verticales des cellules |
| [HasHorizontalBorder](../../aspose.cells.charts/chartdatatable/hashorizontalborder/) { get; set; } | Vrai si le tableau de données du graphique a des bordures horizontales des cellules |
| [HasOutlineBorder](../../aspose.cells.charts/chartdatatable/hasoutlineborder/) { get; set; } | Vrai si le tableau de données du graphique a des bordures extérieures |
| [HasVerticalBorder](../../aspose.cells.charts/chartdatatable/hasverticalborder/) { get; set; } | Vrai si le tableau de données du graphique a des bordures verticales des cellules |
| [ShowLegendKey](../../aspose.cells.charts/chartdatatable/showlegendkey/) { get; set; } | Vrai si la clé de légende de l'étiquette de données est visible. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDataTableDemo
    {
        public static void ChartDataTableExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Obtention de la référence de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajout de valeurs d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Ajout d'un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);

            // Accès à l'instance du graphique nouvellement ajouté
            Chart chart = worksheet.Charts[chartIndex];

            // Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
            chart.NSeries.Add("A1:B3", true);

            // Affichage du tableau de données
            chart.ShowDataTable = true;

            // Obtention du tableau de données du graphique
            ChartDataTable chartTable = chart.ChartDataTable;

            // Définition des propriétés du tableau de données du graphique
            chartTable.Font.Color = Color.Red;
            chartTable.AutoScaleFont = true;
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.HasBorderOutline = true;
            chartTable.ShowLegendKey = false;

            // Enregistrement du fichier Excel
            workbook.Save("ChartDataTableExample.xlsx");
            workbook.Save("ChartDataTableExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


