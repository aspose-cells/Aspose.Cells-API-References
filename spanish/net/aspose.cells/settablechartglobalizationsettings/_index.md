---
title: "Clase SettableChartGlobalizationSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.SettableChartGlobalizationSettings. Implementación de PivotGlobalizationSettings que permite al usuario establecer/cambiar textos predefinidos"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/
---
## SettableChartGlobalizationSettings class

Implementación de PivotGlobalizationSettings que permite al usuario establecer/cambiar textos predefinidos.

```csharp
public class SettableChartGlobalizationSettings : ChartGlobalizationSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SettableChartGlobalizationSettings](settablechartglobalizationsettings/)() | El constructor predeterminado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [GetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/getaxistitlename/)() | Obtiene el nombre del título para el eje |
| override [GetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Obtiene el nombre de la unidad del eje |
| override [GetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/getcharttitlename/)() | Obtiene el nombre del título del gráfico |
| override [GetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/)() | Obtiene el nombre de disminución para la leyenda |
| override [GetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegendincreasename/)() | Obtiene el nombre de aumento para la leyenda |
| override [GetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/getlegendtotalname/)() | Obtiene el nombre de total para la leyenda |
| override [GetOtherName](../../aspose.cells/settablechartglobalizationsettings/getothername/)() | Obtiene el nombre de las etiquetas "Other" para el gráfico |
| override [GetSeriesName](../../aspose.cells/settablechartglobalizationsettings/getseriesname/)() | Obtiene el nombre de la serie en el gráfico |
| [SetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/setaxistitlename/)(string) | Establece el nombre del título para el eje |
| [SetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/setaxisunitname/)(DisplayUnitType, string) | Establece el nombre de la unidad del eje |
| [SetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/setcharttitlename/)(string) | Establece el nombre del título del gráfico |
| [SetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/)(string) | Establece el nombre de disminución para la leyenda |
| [SetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegendincreasename/)(string) | Establece el nombre de aumento para la leyenda |
| [SetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/setlegendtotalname/)(string) | Establece el nombre de total para la leyenda |
| [SetOtherName](../../aspose.cells/settablechartglobalizationsettings/setothername/)(string) | Establece el nombre de las etiquetas "Other" para el gráfico |
| [SetSeriesName](../../aspose.cells/settablechartglobalizationsettings/setseriesname/)(string) | Establece el nombre de la serie en el gráfico |

### Ejemplos

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
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una instancia de SettableChartGlobalizationSettings
                var settings = new SettableChartGlobalizationSettings();

                // Establecer configuraciones de globalización personalizadas
                settings.SetSeriesName("Custom Series");
                settings.SetChartTitleName("Custom Chart Title");
                settings.SetLegendIncreaseName("Custom Increase");
                settings.SetLegendDecreaseName("Custom Decrease");

                // Crear una implementación personalizada de GlobalizationSettings
                workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings(settings);

                // Crear un gráfico sencillo para demostrar las configuraciones
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

            // Implementar aquí los métodos requeridos de GlobalizationSettings
            // que delega a la instancia SettableChartGlobalizationSettings
        }
    }
}
```

### Ver también

* class [ChartGlobalizationSettings](../../aspose.cells.charts/chartglobalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


