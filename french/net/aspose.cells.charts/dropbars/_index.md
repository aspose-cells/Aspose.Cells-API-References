---
title: "Classe DropBars"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.DropBars class. Représente les barres haut et bas dans un graphique"
type: docs
url: /fr/net/aspose.cells.charts/dropbars/
---
## DropBars class

Représente les barres haut et bas dans un graphique.

```csharp
public class DropBars
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Area](../../aspose.cells.charts/dropbars/area/) { get; } | Obtient le [`Area`](./area/). |
| [Border](../../aspose.cells.charts/dropbars/border/) { get; } | Obtient la bordure [`Line`](../../aspose.cells.drawing/line/). |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DropBarsDemo
    {
        public static void DropBarsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajoutez NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
            chart.NSeries.Add("A1:B3", true);

            // Activer les barres haut et bas
            chart.NSeries[0].HasUpDownBars = true;

            // Accéder à l'objet DropBars
            DropBars upBars = chart.NSeries[0].UpBars;
            DropBars downBars = chart.NSeries[0].DownBars;

            // Personnaliser l'apparence des barres haut
            upBars.Border.Color = Color.Green;
            upBars.Area.ForegroundColor = Color.LightGreen;

            // Personnaliser l'apparence des barres bas
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            // Enregistrez le classeur
            workbook.Save("DropBarsExample.xlsx");
            workbook.Save("DropBarsExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


