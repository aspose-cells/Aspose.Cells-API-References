---
title: "ChartDataTable.Font"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartDataTable. Obtient un objet Font qui représente le paramètre de police du tableau de données du graphique spécifié"
type: docs
url: /fr/net/aspose.cells.charts/chartdatatable/font/
---
## ChartDataTable.Font property

Obtient un objet `Font` qui représente le paramètre de police du tableau de données du graphique spécifié.

```csharp
public Font Font { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyFontDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Activer le tableau de données
            chart.ShowDataTable = true;
            
            // Obtenir l’objet tableau de données
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // Personnaliser la police du tableau de données
            dataTable.Font.Size = 14;
            dataTable.Font.Color = Color.Red;
            dataTable.Font.IsBold = true;
            dataTable.Font.Name = "Arial";

            // Enregistrez le classeur
            workbook.Save("ChartDataTableFontDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Font](../../../aspose.cells/font/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


