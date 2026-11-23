---
title: "Enum ChartLineFormattingType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.ChartLineFormattingType enum. Représente le type de format de ligne du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartlineformattingtype/
---
## ChartLineFormattingType enumeration

Représente le type de format de ligne d'une ligne de graphique.

```csharp
public enum ChartLineFormattingType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Automatic | `0` | Représente le type de formatage automatique. |
| Solid | `1` | Représente le type de formatage plein. |
| None | `2` | Représente le type de formatage aucun. |
| Gradient | `3` | Dégradé |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartLineFormattingTypeDemo
    {
        public static void ChartLineFormattingTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter des séries au graphique
            chart.NSeries.Add("A1:B3", true);
            
            // Définir les données de catégorie
            chart.NSeries.CategoryData = "A1:A3";
            
            // Définir différents types de formatage de ligne pour les séries
            chart.NSeries[0].SeriesLines.FormattingType = ChartLineFormattingType.Solid;
            chart.NSeries[0].SeriesLines.Color = Color.Red;
            
            // Ajouter une autre série avec un formatage différent
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
            chart.NSeries[1].SeriesLines.Color = Color.Blue;
            
            // Enregistrez le classeur
            workbook.Save("ChartLineFormattingTypeExample.xlsx");
            workbook.Save("ChartLineFormattingTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


