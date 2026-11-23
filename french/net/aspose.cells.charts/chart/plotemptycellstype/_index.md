---
title: "Chart.PlotEmptyCellsType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Obtient et définit comment tracer les cellules vides"
type: docs
url: /fr/net/aspose.cells.charts/chart/plotemptycellstype/
---
## Chart.PlotEmptyCellsType property

Obtient et définit comment tracer les cellules vides.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotEmptyCellsTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple avec quelques cellules vides
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            // B3 est laissé vide
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la plage de données
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Démontrer la propriété PlotEmptyCellsType
            chart.PlotEmptyCellsType = Aspose.Cells.Charts.PlotEmptyCellsType.Zero;
            Console.WriteLine("PlotEmptyCellsType set to: " + chart.PlotEmptyCellsType);

            // Enregistrez le classeur
            workbook.Save("PlotEmptyCellsTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


