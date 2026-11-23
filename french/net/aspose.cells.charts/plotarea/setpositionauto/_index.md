---
title: "PlotArea.SetPositionAuto"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PlotArea. Définir la position de la zone du graphique sur automatique"
type: docs
url: /fr/net/aspose.cells.charts/plotarea/setpositionauto/
---
## PlotArea.SetPositionAuto method

Définir la position de la zone de tracé sur automatique

```csharp
public override void SetPositionAuto()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaMethodSetPositionAutoDemo
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

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Obtenir la zone de tracé du graphique
                PlotArea plotArea = chart.PlotArea;
                
                // Définissez manuellement d'abord quelques valeurs de position pour démontrer l'effet
                plotArea.XRatioToChart = 0.1;
                plotArea.YRatioToChart = 0.1;
                plotArea.WidthRatioToChart = 0.8;
                plotArea.HeightRatioToChart = 0.8;
                
                // Appelez SetPositionAuto pour réinitialiser le positionnement automatique
                plotArea.SetPositionAuto();
                
                Console.WriteLine("Plot area position has been set to automatic.");
                
                // Enregistrer le classeur pour montrer l'effet
                workbook.Save("PlotAreaSetPositionAutoDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPositionAuto method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


