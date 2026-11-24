---
title: "Klasse SettableChartGlobalizationSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.SettableChartGlobalizationSettings Klasse. Implementierung von PivotGlobalizationSettings, die es dem Benutzer ermöglicht, vordefinierte Texte zu setzen/zu ändern"
type: docs
url: /de/net/aspose.cells/settablechartglobalizationsettings/
---
## SettableChartGlobalizationSettings class

Implementierung von PivotGlobalizationSettings, die es dem Benutzer ermöglicht, vordefinierte Texte festzulegen/zu ändern.

```csharp
public class SettableChartGlobalizationSettings : ChartGlobalizationSettings
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SettableChartGlobalizationSettings](settablechartglobalizationsettings/)() | Der Standardkonstruktor. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [GetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/getaxistitlename/)() | Liefert den Namen des Titels für die Achse. |
| override [GetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Liefert den Namen der Achseneinheit. |
| override [GetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/getcharttitlename/)() | Liefert den Namen des Diagrammtitels. |
| override [GetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/)() | Liefert den Namen für 'Abnahme' in der Legende. |
| override [GetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegendincreasename/)() | Liefert den Namen für 'Zunahme' in der Legende. |
| override [GetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/getlegendtotalname/)() | Ermittelt den Namen von Total für die Legende. |
| override [GetOtherName](../../aspose.cells/settablechartglobalizationsettings/getothername/)() | Ermittelt den Namen der "Other"-Beschriftungen für das Diagramm. |
| override [GetSeriesName](../../aspose.cells/settablechartglobalizationsettings/getseriesname/)() | Ermittelt den Namen der Serie im Diagramm. |
| [SetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/setaxistitlename/)(string) | Setzt den Namen des Titels für die Achse. |
| [SetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/setaxisunitname/)(DisplayUnitType, string) | Setzt den Namen der Achseneinheit. |
| [SetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/setcharttitlename/)(string) | Setzt den Namen des Diagrammtitels. |
| [SetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/)(string) | Setzt den Namen von Decrease für die Legende. |
| [SetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegendincreasename/)(string) | Setzt den Namen von increase für die Legende. |
| [SetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/setlegendtotalname/)(string) | Setzt den Namen von Total für die Legende. |
| [SetOtherName](../../aspose.cells/settablechartglobalizationsettings/setothername/)(string) | Setzt den Namen der "Other"-Beschriftungen für das Diagramm. |
| [SetSeriesName](../../aspose.cells/settablechartglobalizationsettings/setseriesname/)(string) | Setzt den Namen der Serie im Diagramm. |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstelle eine Instanz von SettableChartGlobalizationSettings
                var settings = new SettableChartGlobalizationSettings();

                // Benutzerdefinierte Globalisierungseinstellungen festlegen
                settings.SetSeriesName("Custom Series");
                settings.SetChartTitleName("Custom Chart Title");
                settings.SetLegendIncreaseName("Custom Increase");
                settings.SetLegendDecreaseName("Custom Decrease");

                // Erstelle eine benutzerdefinierte Implementierung von GlobalizationSettings
                workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings(settings);

                // Erstelle ein einfaches Diagramm, um die Einstellungen zu demonstrieren
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

            // Implementiere hier die erforderlichen GlobalizationSettings-Methoden
            // die an die SettableChartGlobalizationSettings-Instanz delegieren
        }
    }
}
```

### Siehe auch

* class [ChartGlobalizationSettings](../../aspose.cells.charts/chartglobalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


