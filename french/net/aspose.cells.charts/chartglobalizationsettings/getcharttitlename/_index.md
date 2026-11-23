---
title: "ChartGlobalizationSettings.GetChartTitleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ChartGlobalizationSettings. Obtient le nom du titre du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartglobalizationsettings/getcharttitlename/
---
## ChartGlobalizationSettings.GetChartTitleName method

Obtient le nom de Chart Title

```csharp
public virtual string GetChartTitleName()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetChartTitleNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un graphique d'exemple à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Créer une instance de ChartGlobalizationSettings
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();

            // Démontrer l'utilisation de la méthode GetChartTitleName
            string chartTitleName = globalizationSettings.GetChartTitleName();
            Console.WriteLine("Chart Title Name: " + chartTitleName);

            // Enregistrez le classeur
            workbook.Save("ChartGlobalizationSettingsExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


