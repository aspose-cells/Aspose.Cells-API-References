---
title: "Line.WeightPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Obtient ou définit le poids de la ligne en pixels"
type: docs
url: /fr/net/aspose.cells.drawing/line/weightpx/
---
## Line.WeightPx property

Obtient ou définit le poids de la ligne en unités de pixels.

```csharp
public double WeightPx { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightPxDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Ajoutez des données d'exemple
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].PutValue(15);
            cells["B2"].PutValue(25);
            cells["B3"].PutValue(35);

            // Ajouter un graphique linéaire
            int chartIndex = workbook.Worksheets[0].Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurer les propriétés de ligne avec WeightPx
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Border.WeightPx = 5.0; // Set line weight in pixels
            series.Border.Color = System.Drawing.Color.Blue;

            // Enregistrez le classeur
            workbook.Save("LineWeightPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


