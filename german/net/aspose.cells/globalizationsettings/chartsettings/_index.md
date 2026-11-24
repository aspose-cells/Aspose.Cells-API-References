---
title: "GlobalizationSettings.ChartSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Eigenschaft. Gibt die Globalisierungseinstellungen für Chart zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/globalizationsettings/chartsettings/
---
## GlobalizationSettings.ChartSettings property

Liest oder legt die Globalisierungseinstellungen für Diagramme fest.

```csharp
public ChartGlobalizationSettings ChartSettings { get; set; }
```

### Beispiele

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
            
            // Ein Diagramm erstellen
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = sheet.Charts[chartIndex];
            
            // Fügen Sie Beispieldaten hinzu
            chart.NSeries.Add("{10,20,30,40}", true);
            
            // Anzeigeeinheiten festlegen
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            Console.WriteLine("Default display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Benutzerdefinierte Globalisierungseinstellungen anwenden
            wb.Settings.GlobalizationSettings = new GlobalizationSettings
            {
                ChartSettings = new CustomChartGlobalizationSettings()
            };
            
            // Die benutzerdefinierten Beschriftungen überprüfen
            Console.WriteLine("Custom display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Anzeigeeinheit ändern und überprüfen
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            Console.WriteLine("Updated display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
        }
    }
}
```

### Siehe auch

* class [ChartGlobalizationSettings](../../../aspose.cells.charts/chartglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


