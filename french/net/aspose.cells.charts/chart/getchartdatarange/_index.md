---
title: "Chart.GetChartDataRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Chart. Obtient la plage de source de données du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/getchartdatarange/
---
## Chart.GetChartDataRange method

Obtient la plage de source de données du graphique.

```csharp
public string GetChartDataRange()
```

### Valeur de retour

La source de données.

### Remarques

Prend uniquement en charge les plages. Si les Series.Values, Name et XValues se trouvent dans une plage continue, une plage les contenant sera renvoyée.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodGetChartDataRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C4"].PutValue(60);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("=Sheet1!$B$1:$C$4", true);
            
            // Obtenir et afficher la plage de données du graphique
            string dataRange = chart.GetChartDataRange();
            Console.WriteLine("Chart Data Range: " + dataRange);
            
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


