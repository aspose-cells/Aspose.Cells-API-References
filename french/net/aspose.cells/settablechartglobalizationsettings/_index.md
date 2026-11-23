---
title: "Classe SettableChartGlobalizationSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.SettableChartGlobalizationSettings. Implémentation de PivotGlobalizationSettings qui permet à l'utilisateur de définir/modifier les textes prédéfinis"
type: docs
url: /fr/net/aspose.cells/settablechartglobalizationsettings/
---
## SettableChartGlobalizationSettings class

Implémentation de PivotGlobalizationSettings qui permet à l'utilisateur de définir/modifier des textes prédéfinis.

```csharp
public class SettableChartGlobalizationSettings : ChartGlobalizationSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SettableChartGlobalizationSettings](settablechartglobalizationsettings/)() | Le constructeur par défaut. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [GetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/getaxistitlename/)() | Obtient le nom du Title pour l'axe |
| override [GetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Obtient le nom de Axis Unit |
| override [GetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/getcharttitlename/)() | Obtient le nom de Chart Title |
| override [GetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/)() | Obtient le nom de Decrease pour la légende |
| override [GetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegendincreasename/)() | Obtient le nom de increase pour la légende |
| override [GetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/getlegendtotalname/)() | Obtient le nom de Total pour la légende |
| override [GetOtherName](../../aspose.cells/settablechartglobalizationsettings/getothername/)() | Obtient le nom des libellés "Other" pour le graphique |
| override [GetSeriesName](../../aspose.cells/settablechartglobalizationsettings/getseriesname/)() | Obtient le nom de Series dans le graphique |
| [SetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/setaxistitlename/)(string) | Définit le nom du Title pour l'axe |
| [SetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/setaxisunitname/)(DisplayUnitType, string) | Définit le nom de Axis Unit |
| [SetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/setcharttitlename/)(string) | Définit le nom de Chart Title |
| [SetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/)(string) | Définit le nom de Decrease pour la légende |
| [SetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegendincreasename/)(string) | Définit le nom de increase pour la légende |
| [SetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/setlegendtotalname/)(string) | Définit le nom de Total pour la légende |
| [SetOtherName](../../aspose.cells/settablechartglobalizationsettings/setothername/)(string) | Définit le nom des libellés "Other" pour le graphique |
| [SetSeriesName](../../aspose.cells/settablechartglobalizationsettings/setseriesname/)(string) | Définit le nom de Series dans le graphique |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CellsClassSettableChartGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créer une instance de SettableChartGlobalizationSettings
                var settings = new SettableChartGlobalizationSettings();

                // Définir des paramètres de globalisation personnalisés
                settings.SetSeriesName("Custom Series");
                settings.SetChartTitleName("Custom Chart Title");
                settings.SetLegendIncreaseName("Custom Increase");
                settings.SetLegendDecreaseName("Custom Decrease");

                // Créer une implémentation personnalisée de GlobalizationSettings
                workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings(settings);

                // Créer un graphique simple pour démontrer les paramètres
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Q1");
                worksheet.Cells["A3"].PutValue("Q2");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);

                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";
                chart.Title.Text = "Demo Chart";

                Console.WriteLine("SettableChartGlobalizationSettings configured successfully");
                workbook.Save("SettableChartGlobalizationSettingsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SettableChartGlobalizationSettings: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            private readonly SettableChartGlobalizationSettings _chartSettings;

            public CustomGlobalizationSettings(SettableChartGlobalizationSettings chartSettings)
            {
                _chartSettings = chartSettings;
            }

            // Implémenter ici les méthodes requises de GlobalizationSettings
            // qui délègue à l'instance SettableChartGlobalizationSettings
        }
    }
}
```

### Voir aussi

* class [ChartGlobalizationSettings](../../aspose.cells.charts/chartglobalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


