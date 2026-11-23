---
title: "TickLabels.ReadingOrder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TickLabels. Représente l'ordre de lecture du texte"
type: docs
url: /fr/net/aspose.cells.charts/ticklabels/readingorder/
---
## TickLabels.ReadingOrder property

Représente l'ordre de lecture du texte.

```csharp
public TextDirectionType ReadingOrder { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyReadingOrderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Définir l'ordre de lecture des libellés d'échelle
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.ReadingOrder = TextDirectionType.RightToLeft;

            // Enregistrez le classeur
            workbook.Save("TickLabelsReadingOrderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


