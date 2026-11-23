---
title: "Énumération PlotEmptyCellsType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.PlotEmptyCellsType enum. Représente tous les types de cellules vides du tracé d'un graphique"
type: docs
url: /fr/net/aspose.cells.charts/plotemptycellstype/
---
## PlotEmptyCellsType enumeration

Représente tous les types de cellules vides du tracé d'un graphique.

```csharp
public enum PlotEmptyCellsType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| NotPlotted | `0` | Non tracé (laisser un espace) |
| Zero | `1` | Zéro |
| Interpolated | `2` | Interpolé |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotEmptyCellsTypeDemo
    {
        public static void PlotEmptyCellsTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(null); // Empty cell
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données pour le graphique
            chart.SetChartDataRange("A1:B5", true);

            // Définir le titre du graphique
            chart.Title.Text = "Plot Empty Cells Example";

            // Définir comment tracer les cellules vides
            chart.PlotEmptyCellsType = PlotEmptyCellsType.Interpolated;

            // Enregistrez le classeur
            workbook.Save("PlotEmptyCellsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


