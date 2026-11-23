---
title: "Chart.ValueAxis"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété du graphique. Obtient l'axe Y du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/valueaxis/
---
## Chart.ValueAxis property

Obtient l'axe Y du graphique.

```csharp
public Axis ValueAxis { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyValueAxisDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100000000);
            worksheet.Cells["B3"].PutValue(200000000);
            worksheet.Cells["B4"].PutValue(300000000);

            // Ajouter un graphique et définir sa plage de données
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurer les propriétés de ValueAxis
            chart.ValueAxis.DisplayUnit = DisplayUnitType.HundredMillions;
            chart.ValueAxis.Title.Text = "Values (in 100 millions)";
            chart.ValueAxis.MajorUnit = 1;

            // Enregistrez le classeur
            workbook.Save("ChartPropertyValueAxisDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


