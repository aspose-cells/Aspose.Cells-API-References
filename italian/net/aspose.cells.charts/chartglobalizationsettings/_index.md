---
title: "Classe ChartGlobalizationSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.ChartGlobalizationSettings. Rappresenta le impostazioni di globalizzazione per un grafico"
type: docs
url: /it/net/aspose.cells.charts/chartglobalizationsettings/
---
## ChartGlobalizationSettings class

Rappresenta le impostazioni di globalizzazione per un grafico.

```csharp
public class ChartGlobalizationSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ChartGlobalizationSettings](chartglobalizationsettings/)() | Il costruttore predefinito. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [GetAxisTitleName](../../aspose.cells.charts/chartglobalizationsettings/getaxistitlename/)() | Ottiene il nome del Titolo per l'Asse. |
| virtual [GetAxisUnitName](../../aspose.cells.charts/chartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Ottiene il nome dell'Unità dell'Asse. |
| virtual [GetChartTitleName](../../aspose.cells.charts/chartglobalizationsettings/getcharttitlename/)() | Ottiene il nome del Titolo del Grafico. |
| virtual [GetLegendDecreaseName](../../aspose.cells.charts/chartglobalizationsettings/getlegenddecreasename/)() | Ottiene il nome di Diminuzione per la Legenda. |
| virtual [GetLegendIncreaseName](../../aspose.cells.charts/chartglobalizationsettings/getlegendincreasename/)() | Ottiene il nome di Aumento per la Legenda. |
| virtual [GetLegendTotalName](../../aspose.cells.charts/chartglobalizationsettings/getlegendtotalname/)() | Ottiene il nome di Totale per la Legenda. |
| virtual [GetOtherName](../../aspose.cells.charts/chartglobalizationsettings/getothername/)() | Ottiene il nome delle etichette "Altro" per il Grafico. |
| virtual [GetSeriesName](../../aspose.cells.charts/chartglobalizationsettings/getseriesname/)() | Ottiene il nome della Serie nel Grafico. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartGlobalizationSettingsDemo
    {
        public static void ChartGlobalizationSettingsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un grafico di esempio al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Crea un'istanza di ChartGlobalizationSettings
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();

            // Dimostra l'uso dei metodi in ChartGlobalizationSettings
            string seriesName = globalizationSettings.GetSeriesName();
            string chartTitleName = globalizationSettings.GetChartTitleName();
            string legendIncreaseName = globalizationSettings.GetLegendIncreaseName();
            string legendDecreaseName = globalizationSettings.GetLegendDecreaseName();
            string legendTotalName = globalizationSettings.GetLegendTotalName();
            string axisTitleName = globalizationSettings.GetAxisTitleName();
            string otherName = globalizationSettings.GetOtherName();
            string axisUnitName = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);

            // Stampa i nomi recuperati sulla console
            Console.WriteLine("Series Name: " + seriesName);
            Console.WriteLine("Chart Title Name: " + chartTitleName);
            Console.WriteLine("Legend Increase Name: " + legendIncreaseName);
            Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);
            Console.WriteLine("Legend Total Name: " + legendTotalName);
            Console.WriteLine("Axis Title Name: " + axisTitleName);
            Console.WriteLine("Other Name: " + otherName);
            Console.WriteLine("Axis Unit Name: " + axisUnitName);

            // Salva la cartella di lavoro
            workbook.Save("ChartGlobalizationSettingsExample.xlsx");
            workbook.Save("ChartGlobalizationSettingsExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


