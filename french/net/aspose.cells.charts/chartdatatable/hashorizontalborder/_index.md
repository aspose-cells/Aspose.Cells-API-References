---
title: "ChartDataTable.HasHorizontalBorder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartDataTable. True si le tableau de données du graphique possède des bordures de cellules horizontales"
type: docs
url: /fr/net/aspose.cells.charts/chartdatatable/hashorizontalborder/
---
## ChartDataTable.HasHorizontalBorder property

Vrai si le tableau de données du graphique a des bordures horizontales des cellules

```csharp
public bool HasHorizontalBorder { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasHorizontalBorderDemo
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

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Activer le tableau de données
            chart.ShowDataTable = true;
            // Obtenez le tableau de données via la propriété ChartDataTable
            ChartDataTable dataTable = chart.ChartDataTable;

            // Démontrer la propriété HasHorizontalBorder
            dataTable.HasHorizontalBorder = true;
            Console.WriteLine("DataTable HasHorizontalBorder: " + dataTable.HasHorizontalBorder);

            // Enregistrez le classeur
            workbook.Save("ChartDataTablePropertyHasHorizontalBorderDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


