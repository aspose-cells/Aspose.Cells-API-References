---
title: "Chart.ChartDataTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Chart property. Représente le tableau de données du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/chartdatatable/
---
## Chart.ChartDataTable property

Représente le tableau de données du graphique.

```csharp
public ChartDataTable ChartDataTable { get; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyChartDataTableDemo
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
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";

            // Activer et personnaliser le tableau de données
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Définir les propriétés du tableau de données
            dataTable.ShowLegendKey = true;
            dataTable.HasBorderHorizontal = true;
            dataTable.HasBorderVertical = true;
            dataTable.HasBorderOutline = true;
            dataTable.AutoScaleFont = true;
            dataTable.BackgroundMode = BackgroundMode.Opaque;

            // Personnaliser la police du tableau de données
            dataTable.Font.Name = "Arial";
            dataTable.Font.Size = 10;
            dataTable.Font.Color = Color.Blue;
            dataTable.Font.IsBold = true;

            // Personnaliser les bordures du tableau de données
            dataTable.Border.Color = Color.Red;
            dataTable.Border.Style = LineType.Dash;
            dataTable.Border.Weight = WeightType.MediumLine;

            // Enregistrez le classeur
            workbook.Save("ChartDataTableDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartDataTable](../../chartdatatable/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


