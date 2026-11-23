---
title: "SeriesLayoutProperties.Subtotals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SeriesLayoutProperties. Représente l'index d'un point de données de sous-total"
type: docs
url: /fr/net/aspose.cells.charts/serieslayoutproperties/subtotals/
---
## SeriesLayoutProperties.Subtotals property

Représente l'index d'un point de données de sous-total.

```csharp
public int[] Subtotals { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertySubtotalsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définissez les sous-totaux pour la première série
            chart.NSeries[0].LayoutProperties.Subtotals = new int[] { 0, 3 };

            // Vérifiez que les sous-totaux ont été définis correctement
            Console.WriteLine("Subtotal at index 0: " + chart.NSeries[0].LayoutProperties.Subtotals[0]);
            Console.WriteLine("Subtotal at index 1: " + chart.NSeries[0].LayoutProperties.Subtotals[1]);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


