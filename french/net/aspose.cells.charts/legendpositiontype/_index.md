---
title: "Enum LegendPositionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.LegendPositionType enum. Énumère les types de position de la légende"
type: docs
url: /fr/net/aspose.cells.charts/legendpositiontype/
---
## LegendPositionType enumeration

Énumère les types de position de la légende.

```csharp
public enum LegendPositionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Bottom | `0` | Affiche la légende en bas de la zone de tracé du graphique. |
| Corner | `1` | Affiche la légende dans le coin de la zone de tracé du graphique. |
| Left | `4` | Affiche la légende à gauche de la zone de tracé du graphique. |
| NotDocked | `7` | Indique que la légende n'est pas ancrée. |
| Right | `3` | Affiche la légende à droite de la zone de tracé du graphique. |
| Top | `2` | Affiche la légende en haut de la zone de tracé du graphique. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPositionTypeDemo
    {
        public static void LegendPositionTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Ajoutez un graphique en colonnes à la feuille de calcul
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Accédez à la légende du graphique
            Legend legend = chart.Legend;

            // Définir la position de la légende à gauche du graphique
            legend.Position = LegendPositionType.Left;

            // Définir des propriétés supplémentaires pour la légende
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;

            // Enregistrez le classeur
            workbook.Save("LegendPositionTypeExample.xlsx");
            workbook.Save("LegendPositionTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


