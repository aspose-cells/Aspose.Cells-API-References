---
title: "ChartGlobalizationSettings.GetLegendTotalName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ChartGlobalizationSettings. Obtient le nom du total pour la légende"
type: docs
url: /fr/net/aspose.cells.charts/chartglobalizationsettings/getlegendtotalname/
---
## ChartGlobalizationSettings.GetLegendTotalName method

Obtient le nom de Total pour la légende

```csharp
public virtual string GetLegendTotalName()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetLegendTotalNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Créer les paramètres de mondialisation et obtenir le nom du total de la légende
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string legendTotalName = globalizationSettings.GetLegendTotalName();

            // Afficher le résultat
            Console.WriteLine("Legend Total Name: " + legendTotalName);

            // Enregistrer le classeur
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


