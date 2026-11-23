---
title: "Énumération PlotDataByType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Charts.PlotDataByType. Représente le type de tracé de données par ligne ou par colonne"
type: docs
url: /fr/net/aspose.cells.charts/plotdatabytype/
---
## PlotDataByType enumeration

Représente le type de tracé de données par ligne ou colonne.

```csharp
public enum PlotDataByType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Row | `0` | Trié par ligne. |
| Column | `1` | Par colonne. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassPlotDataByTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter des données d'exemple à la feuille de calcul
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value1");
                worksheet.Cells["C1"].PutValue("Value2");
                worksheet.Cells["A2"].PutValue("Row1");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["C2"].PutValue(20);
                worksheet.Cells["A3"].PutValue("Row2");
                worksheet.Cells["B3"].PutValue(30);
                worksheet.Cells["C3"].PutValue(40);

                // Ajouter un graphique à la feuille de calcul
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Définir la plage de données du graphique
                chart.NSeries.Add("B2:C3", true);

                // Démontrer l'utilisation des valeurs de l'énumération PlotDataByType
                PlotDataByType plotType = PlotDataByType.Row;
                Console.WriteLine($"Chart is currently plotting data by: {plotType}");

                // Passer au tracé par colonne
                plotType = PlotDataByType.Column;
                Console.WriteLine($"Chart is now plotting data by: {plotType}");

                // Enregistrez le classeur
                workbook.Save("PlotDataByTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with PlotDataByType demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PlotDataByType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


