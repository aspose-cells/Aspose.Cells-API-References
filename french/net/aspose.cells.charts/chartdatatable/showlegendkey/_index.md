---
title: "ChartDataTable.ShowLegendKey"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartDataTable. Vrai si la clé de légende de l'étiquette de données est visible"
type: docs
url: /fr/net/aspose.cells.charts/chartdatatable/showlegendkey/
---
## ChartDataTable.ShowLegendKey property

Vrai si la clé de légende de l'étiquette de données est visible.

```csharp
public bool ShowLegendKey { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyShowLegendKeyDemo
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

            // Activer le tableau de données avec la clé de légende
            chart.ShowDataTable = true;
            // Accéder à DataTable via les propriétés du graphique
            if (chart.ChartDataTable != null)
            {
                chart.ChartDataTable.ShowLegendKey = true;
            }

            // Enregistrez le classeur
            workbook.Save("ChartDataTableShowLegendKeyDemo.xlsx");

            Console.WriteLine("Chart created with ShowLegendKey enabled in data table.");
        }
    }
}
```

### Voir aussi

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


