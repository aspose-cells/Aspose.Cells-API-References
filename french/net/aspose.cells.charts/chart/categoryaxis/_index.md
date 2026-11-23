---
title: "Chart.CategoryAxis"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Chart property. Obtient l'axe X du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/categoryaxis/
---
## Chart.CategoryAxis property

Obtient l'axe X du graphique.

```csharp
public Axis CategoryAxis { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyCategoryAxisDemo
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

            // Ajouter un graphique en colonnes
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder et modifier les propriétés de CategoryAxis
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;
            chart.CategoryAxis.Title.Text = "Sample Categories";
            chart.CategoryAxis.Title.Font.Size = 12;

            // Enregistrez le classeur
            workbook.Save("CategoryAxisDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


