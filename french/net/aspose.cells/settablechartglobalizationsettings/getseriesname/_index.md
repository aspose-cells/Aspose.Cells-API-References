---
title: "SettableChartGlobalizationSettings.GetSeriesName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableChartGlobalizationSettings. Obtient le nom des séries dans le graphique"
type: docs
url: /fr/net/aspose.cells/settablechartglobalizationsettings/getseriesname/
---
## SettableChartGlobalizationSettings.GetSeriesName method

Obtient le nom de Series dans le graphique

```csharp
public override string GetSeriesName()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetSeriesNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Column A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Column B");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Créer et appliquer les paramètres de mondialisation
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();
            settings.SetSeriesName("Custom Series Name");
            
            // Les paramètres de mondialisation sont utilisés lors du rendu/affichage du graphique,
            // mais ne sont pas directement assignés à l'objet graphique
            // (car la classe Chart n'a pas cette propriété)

            try
            {
                // Obtenir le nom de série personnalisé
                string seriesName = settings.GetSeriesName();
                Console.WriteLine("Series Name: " + seriesName);

                // Enregistrez le classeur
                workbook.Save("MethodGetSeriesNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSeriesName method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


