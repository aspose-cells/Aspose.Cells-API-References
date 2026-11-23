---
title: "Chart.SetChartDataRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Chart. Spécifie la plage de données pour un graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/setchartdatarange/
---
## Chart.SetChartDataRange method

Spécifie la plage de données pour un graphique.

```csharp
public void SetChartDataRange(string area, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| zone | String | Spécifie les valeurs à partir desquelles tracer la série de données |
| isVertical | Boolean | Spécifie s'il faut tracer la série à partir d'une plage de valeurs de cellules par ligne ou par colonne. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodSetChartDataRangeWithStringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("Cat3");
            worksheet.Cells["B4"].PutValue(30);
            
            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


