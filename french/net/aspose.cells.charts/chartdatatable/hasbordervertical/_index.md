---
title: "ChartDataTable.HasBorderVertical"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartDataTable. True si le tableau de données du graphique possède des bordures de cellules verticales"
type: docs
url: /fr/net/aspose.cells.charts/chartdatatable/hasbordervertical/
---
## ChartDataTable.HasBorderVertical property

Vrai si le tableau de données du graphique a des bordures verticales des cellules

```csharp
[Obsolete("Use ChartDataTable.HasVerticalBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderVertical { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ChartDataTable.HasVerticalBorder. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2024. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasBorderVerticalDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.ShowDataTable = true;

            ChartDataTable chartTable = chart.ChartDataTable;
            chartTable.HasBorderVertical = true;
            chartTable.HasBorderHorizontal = true;

            workbook.Save("ChartDataTable_HasBorderVertical.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


