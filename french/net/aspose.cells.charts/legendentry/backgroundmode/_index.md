---
title: "LegendEntry.BackgroundMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LegendEntry. Obtient et définit le mode d'affichage de l'arrière-plan"
type: docs
url: /fr/net/aspose.cells.charts/legendentry/backgroundmode/
---
## LegendEntry.BackgroundMode property

Obtient et définit le mode d'affichage de l'arrière-plan

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyBackgroundModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B2", true);
            chart.NSeries.CategoryData = "C1:C2";

            // Configurer l'entrée de légende
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;
            legendEntry.BackgroundMode = BackgroundMode.Opaque;
            legendEntry.Font.Color = System.Drawing.Color.Blue;

            workbook.Save("LegendEntryBackgroundModeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


