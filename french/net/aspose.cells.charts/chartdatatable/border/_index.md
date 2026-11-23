---
title: "ChartDataTable.Border"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartDataTable. Retourne un objet Border qui représente la bordure de l'objet"
type: docs
url: /fr/net/aspose.cells.charts/chartdatatable/border/
---
## ChartDataTable.Border property

Renvoie un objet Border qui représente la bordure de l'objet

```csharp
public Line Border { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyBorderDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Afficher le tableau de données
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Configurer les propriétés de la bordure
            Line border = dataTable.Border;
            border.Color = System.Drawing.Color.Blue;
            border.Style = LineType.Solid;
            border.Weight = WeightType.MediumLine;
            border.DashType = MsoLineDashStyle.Solid;
            
            // Configurer la visibilité des bordures du tableau
            dataTable.HasHorizontalBorder = true;
            dataTable.HasVerticalBorder = true;
            dataTable.HasOutlineBorder = true;

            // Enregistrez le classeur
            workbook.Save("ChartDataTableBorderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


