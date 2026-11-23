---
title: "Series.DownBars"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Retourne un objet DropBars qui représente les barres descendantes sur un graphique en ligne. S'applique uniquement aux graphiques en ligne"
type: docs
url: /fr/net/aspose.cells.charts/series/downbars/
---
## Series.DownBars property

Retourne un objet [`DropBars`](../../dropbars/) qui représente les barres descendantes sur un graphique en ligne. S'applique uniquement aux graphiques en ligne.

```csharp
public DropBars DownBars { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDownBarsDemo
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

            // Activer et personnaliser les barres descendantes
            chart.NSeries[0].HasUpDownBars = true;
            DropBars downBars = chart.NSeries[0].DownBars;
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            workbook.Save("DownBarsExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


