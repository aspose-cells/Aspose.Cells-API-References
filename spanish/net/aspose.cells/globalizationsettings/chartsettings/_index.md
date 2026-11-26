---
title: "GlobalizationSettings.ChartSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GlobalizationSettings. Obtiene o establece la configuración de globalización para Chart"
type: docs
url: /es/net/aspose.cells/globalizationsettings/chartsettings/
---
## GlobalizationSettings.ChartSettings property

Obtiene o establece la configuración de globalización para el gráfico.

```csharp
public ChartGlobalizationSettings ChartSettings { get; set; }
```

### Ejemplos

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
            
            // Crear un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = sheet.Charts[chartIndex];
            
            // Agregar datos de ejemplo
            chart.NSeries.Add("{10,20,30,40}", true);
            
            // Establecer unidades de visualización
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            Console.WriteLine("Default display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Aplicar configuraciones de globalización personalizadas
            wb.Settings.GlobalizationSettings = new GlobalizationSettings
            {
                ChartSettings = new CustomChartGlobalizationSettings()
            };
            
            // Verificar las etiquetas personalizadas
            Console.WriteLine("Custom display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Cambiar la unidad de visualización y verificar
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            Console.WriteLine("Updated display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
        }
    }
}
```

### Ver también

* class [ChartGlobalizationSettings](../../../aspose.cells.charts/chartglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


