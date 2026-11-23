---
title: "Chart.RefreshPivotData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Chart. Rafraîchit les données du graphique à partir du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.charts/chart/refreshpivotdata/
---
## Chart.RefreshPivotData method

Actualise les données du graphique à partir du tableau croisé dynamique.

```csharp
public void RefreshPivotData()
```

### Remarques

Nous collecterons les données de la source de données pivot vers le rapport du tableau croisé dynamique. Cette méthode est uniquement utilisée pour rassembler toutes les données dans un graphique pivot.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodRefreshPivotDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple à la première feuille de calcul
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(100);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(200);
            dataSheet.Cells["A4"].PutValue("C");
            dataSheet.Cells["B4"].PutValue(300);

            // Créer un tableau croisé dynamique
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            pivotSheet.PivotTables.Add("A1", dataSheet.Cells["A1:B4"].Name, "PivotTable1");

            // Ajoutez un graphique
            int chartIndex = pivotSheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Aspose.Cells.Charts.Chart chart = pivotSheet.Charts[chartIndex];
            
            // Définir la source de données du graphique croisé dynamique
            chart.PivotSource = "Pivot!PivotTable1";
            
            // Actualiser les données du tableau croisé dynamique dans le graphique
            chart.RefreshPivotData();
            
            // Enregistrez le classeur
            workbook.Save("PivotChartWithRefresh.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


