---
title: "Clase ChartGlobalizationSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.ChartGlobalizationSettings. Representa la configuración de globalización para un gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartglobalizationsettings/
---
## ChartGlobalizationSettings class

Representa la configuración de globalización para un gráfico.

```csharp
public class ChartGlobalizationSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ChartGlobalizationSettings](chartglobalizationsettings/)() | El constructor predeterminado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [GetAxisTitleName](../../aspose.cells.charts/chartglobalizationsettings/getaxistitlename/)() | Obtiene el nombre del título para el eje |
| virtual [GetAxisUnitName](../../aspose.cells.charts/chartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Obtiene el nombre de la unidad del eje |
| virtual [GetChartTitleName](../../aspose.cells.charts/chartglobalizationsettings/getcharttitlename/)() | Obtiene el nombre del título del gráfico |
| virtual [GetLegendDecreaseName](../../aspose.cells.charts/chartglobalizationsettings/getlegenddecreasename/)() | Obtiene el nombre de disminución para la leyenda |
| virtual [GetLegendIncreaseName](../../aspose.cells.charts/chartglobalizationsettings/getlegendincreasename/)() | Obtiene el nombre de aumento para la leyenda |
| virtual [GetLegendTotalName](../../aspose.cells.charts/chartglobalizationsettings/getlegendtotalname/)() | Obtiene el nombre de total para la leyenda |
| virtual [GetOtherName](../../aspose.cells.charts/chartglobalizationsettings/getothername/)() | Obtiene el nombre de las etiquetas "Other" para el gráfico |
| virtual [GetSeriesName](../../aspose.cells.charts/chartglobalizationsettings/getseriesname/)() | Obtiene el nombre de la serie en el gráfico |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un gráfico de ejemplo a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Crear una instancia de ChartGlobalizationSettings
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();

            // Demostrar el uso de los métodos en ChartGlobalizationSettings
            string seriesName = globalizationSettings.GetSeriesName();
            string chartTitleName = globalizationSettings.GetChartTitleName();
            string legendIncreaseName = globalizationSettings.GetLegendIncreaseName();
            string legendDecreaseName = globalizationSettings.GetLegendDecreaseName();
            string legendTotalName = globalizationSettings.GetLegendTotalName();
            string axisTitleName = globalizationSettings.GetAxisTitleName();
            string otherName = globalizationSettings.GetOtherName();
            string axisUnitName = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);

            // Imprimir los nombres recuperados en la consola
            Console.WriteLine("Series Name: " + seriesName);
            Console.WriteLine("Chart Title Name: " + chartTitleName);
            Console.WriteLine("Legend Increase Name: " + legendIncreaseName);
            Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);
            Console.WriteLine("Legend Total Name: " + legendTotalName);
            Console.WriteLine("Axis Title Name: " + axisTitleName);
            Console.WriteLine("Other Name: " + otherName);
            Console.WriteLine("Axis Unit Name: " + axisUnitName);

            // Guarda el libro de trabajo
            workbook.Save("ChartGlobalizationSettingsExample.xlsx");
            workbook.Save("ChartGlobalizationSettingsExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


