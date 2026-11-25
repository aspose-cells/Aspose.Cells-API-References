---
title: "Classe SettableChartGlobalizationSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.SettableChartGlobalizationSettings. Implementazione di PivotGlobalizationSettings che consente all'utente di impostare/modificare i testi predefiniti"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/
---
## SettableChartGlobalizationSettings class

Implementazione di PivotGlobalizationSettings che consente all'utente di impostare/modificare testi predefiniti.

```csharp
public class SettableChartGlobalizationSettings : ChartGlobalizationSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SettableChartGlobalizationSettings](settablechartglobalizationsettings/)() | Il costruttore predefinito. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [GetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/getaxistitlename/)() | Ottiene il nome del Titolo per l'Asse. |
| override [GetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Ottiene il nome dell'Unità dell'Asse. |
| override [GetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/getcharttitlename/)() | Ottiene il nome del Titolo del Grafico. |
| override [GetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/)() | Ottiene il nome di Diminuzione per la Legenda. |
| override [GetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegendincreasename/)() | Ottiene il nome di Aumento per la Legenda. |
| override [GetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/getlegendtotalname/)() | Ottiene il nome di Totale per la Legenda. |
| override [GetOtherName](../../aspose.cells/settablechartglobalizationsettings/getothername/)() | Ottiene il nome delle etichette "Altro" per il Grafico. |
| override [GetSeriesName](../../aspose.cells/settablechartglobalizationsettings/getseriesname/)() | Ottiene il nome della Serie nel Grafico. |
| [SetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/setaxistitlename/)(string) | Imposta il nome del Titolo per l'Asse. |
| [SetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/setaxisunitname/)(DisplayUnitType, string) | Imposta il nome dell'Unità dell'Asse. |
| [SetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/setcharttitlename/)(string) | Imposta il nome del Titolo del Grafico. |
| [SetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/)(string) | Imposta il nome di Diminuzione per la Legenda. |
| [SetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegendincreasename/)(string) | Imposta il nome di Aumento per la Legenda. |
| [SetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/setlegendtotalname/)(string) | Imposta il nome di Totale per la Legenda. |
| [SetOtherName](../../aspose.cells/settablechartglobalizationsettings/setothername/)(string) | Imposta il nome delle etichette "Altro" per il Grafico. |
| [SetSeriesName](../../aspose.cells/settablechartglobalizationsettings/setseriesname/)(string) | Imposta il nome della Serie nel Grafico |

### Esempi

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
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea un'istanza di SettableChartGlobalizationSettings
                var settings = new SettableChartGlobalizationSettings();

                // Imposta impostazioni di globalizzazione personalizzate
                settings.SetSeriesName("Custom Series");
                settings.SetChartTitleName("Custom Chart Title");
                settings.SetLegendIncreaseName("Custom Increase");
                settings.SetLegendDecreaseName("Custom Decrease");

                // Crea un'implementazione personalizzata di GlobalizationSettings
                workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings(settings);

                // Crea un grafico semplice per dimostrare le impostazioni
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

            // Implementa qui i metodi richiesti di GlobalizationSettings
            // che delega all'istanza SettableChartGlobalizationSettings
        }
    }
}
```

### Vedi anche

* class [ChartGlobalizationSettings](../../aspose.cells.charts/chartglobalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


