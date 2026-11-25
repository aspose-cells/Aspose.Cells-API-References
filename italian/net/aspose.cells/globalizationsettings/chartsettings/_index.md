---
title: "GlobalizationSettings.ChartSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GlobalizationSettings. Ottiene o imposta le impostazioni di globalizzazione per Chart"
type: docs
url: /it/net/aspose.cells/globalizationsettings/chartsettings/
---
## GlobalizationSettings.ChartSettings property

Ottiene o imposta le impostazioni di globalizzazione per il grafico.

```csharp
public ChartGlobalizationSettings ChartSettings { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class CustomChartGlobalizationSettings : ChartGlobalizationSettings
    {
        public override string GetAxisUnitName(DisplayUnitType type)
        {
            switch (type)
            {
                case DisplayUnitType.Hundreds:
                    return "百";
                case DisplayUnitType.Thousands:
                    return "千";
                case DisplayUnitType.TenThousands:
                    return "万";
                default:
                    return base.GetAxisUnitName(type);
            }
        }
    }

    public class GlobalizationSettingsPropertyChartSettingsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Crea un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = sheet.Charts[chartIndex];
            
            // Aggiungi dati di esempio
            chart.NSeries.Add("{10,20,30,40}", true);
            
            // Imposta le unità di visualizzazione
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            Console.WriteLine("Default display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Applica impostazioni di globalizzazione personalizzate
            wb.Settings.GlobalizationSettings = new GlobalizationSettings
            {
                ChartSettings = new CustomChartGlobalizationSettings()
            };
            
            // Verifica le etichette personalizzate
            Console.WriteLine("Custom display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Modifica l'unità di visualizzazione e verifica
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            Console.WriteLine("Updated display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
        }
    }
}
```

### Vedi anche

* class [ChartGlobalizationSettings](../../../aspose.cells.charts/chartglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


