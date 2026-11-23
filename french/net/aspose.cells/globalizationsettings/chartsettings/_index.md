---
title: "GlobalizationSettings.ChartSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GlobalizationSettings. Obtient ou définit les paramètres de mondialisation pour le graphique"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/chartsettings/
---
## GlobalizationSettings.ChartSettings property

Obtient ou définit les paramètres de mondialisation pour le graphique.

```csharp
public ChartGlobalizationSettings ChartSettings { get; set; }
```

### Exemples

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
            
            // Créer un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ajoutez des données d'exemple
            chart.NSeries.Add("{10,20,30,40}", true);
            
            // Définir les unités d'affichage
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            Console.WriteLine("Default display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Appliquer des paramètres de mondialisation personnalisés
            wb.Settings.GlobalizationSettings = new GlobalizationSettings
            {
                ChartSettings = new CustomChartGlobalizationSettings()
            };
            
            // Vérifier les libellés personnalisés
            Console.WriteLine("Custom display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Modifier l'unité d'affichage et vérifier
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            Console.WriteLine("Updated display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
        }
    }
}
```

### Voir aussi

* class [ChartGlobalizationSettings](../../../aspose.cells.charts/chartglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


