---
title: "Series.UpBars"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété de la série. Retourne un objet DropBars qui représente les barres ascendantes sur un graphique en ligne. S'applique uniquement aux graphiques en ligne"
type: docs
url: /fr/net/aspose.cells.charts/series/upbars/
---
## Series.UpBars property

Renvoie un objet DropBars qui représente les barres ascendantes sur un graphique en lignes. S'applique uniquement aux graphiques en lignes.

```csharp
public DropBars UpBars { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyUpBarsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exemple de données pour un graphique en ligne avec des barres haut/bas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Activer et personnaliser les barres ascendantes
            chart.NSeries[0].HasUpDownBars = true;
            DropBars upBars = chart.NSeries[0].UpBars;
            upBars.Area.ForegroundColor = Color.LightGreen;
            upBars.Border.Color = Color.Green;

            workbook.Save("UpBarsExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


