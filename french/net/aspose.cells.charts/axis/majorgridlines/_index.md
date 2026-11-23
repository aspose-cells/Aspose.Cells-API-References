---
title: "Axis.MajorGridLines"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Représente les lignes de grille majeures sur un axe de graphique"
type: docs
url: /fr/net/aspose.cells.charts/axis/majorgridlines/
---
## Axis.MajorGridLines property

Représente les lignes de grille majeures sur un axe de graphique.

```csharp
public Line MajorGridLines { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorGridLinesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurer les lignes de grille majeures
            chart.ValueAxis.MajorGridLines.IsVisible = false;
            chart.CategoryAxis.MajorGridLines.IsVisible = true;
            chart.CategoryAxis.MajorGridLines.Color = Color.Red;

            // Enregistrez le classeur
            workbook.Save("AxisPropertyMajorGridLinesDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


