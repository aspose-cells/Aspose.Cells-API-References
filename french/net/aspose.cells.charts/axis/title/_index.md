---
title: "Axis.Title"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Obtient le titre de cet axe dans le graphique"
type: docs
url: /fr/net/aspose.cells.charts/axis/title/
---
## Axis.Title property

Obtient le titre de cet axe dans le graphique.

```csharp
public Title Title { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTitleDemo
    {
        public static void Run()
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
            
            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Configurer les titres
            chart.Title.Text = "Sample Chart";
            chart.Title.IsVisible = true;
            chart.Title.Font.Name = "Arial";
            chart.Title.Font.Size = 14;
            
            // Configurer les titres d'axe
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.IsVisible = true;
            chart.CategoryAxis.Title.Font.Name = "Arial";
            
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.IsVisible = true;
            chart.ValueAxis.Title.Font.Name = "Arial";
            
            // Enregistrez le classeur
            workbook.Save("AxisPropertyTitleDemo_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Title](../../title/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


