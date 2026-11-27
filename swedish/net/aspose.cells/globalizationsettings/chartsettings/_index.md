---
title: "GlobalizationSettings.ChartSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-egenskap. Hämtar eller anger globaliseringsinställningarna för diagram"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/chartsettings/
---
## GlobalizationSettings.ChartSettings property

Hämtar eller anger globaliseringsinställningarna för diagram.

```csharp
public ChartGlobalizationSettings ChartSettings { get; set; }
```

### Exempel

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
            
            // Skapa ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = sheet.Charts[chartIndex];
            
            // Lägg till exempeldata
            chart.NSeries.Add("{10,20,30,40}", true);
            
            // Ställ in visningsenheter
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            Console.WriteLine("Default display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Tillämpa anpassade globaliseringsinställningar
            wb.Settings.GlobalizationSettings = new GlobalizationSettings
            {
                ChartSettings = new CustomChartGlobalizationSettings()
            };
            
            // Verifiera de anpassade etiketterna
            Console.WriteLine("Custom display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Ändra displayenhet och verifiera
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            Console.WriteLine("Updated display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
        }
    }
}
```

### Se även

* class [ChartGlobalizationSettings](../../../aspose.cells.charts/chartglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


