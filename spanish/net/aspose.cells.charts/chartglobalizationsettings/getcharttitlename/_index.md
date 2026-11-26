---
title: "ChartGlobalizationSettings.GetChartTitleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartGlobalizationSettings. Obtiene el nombre del título del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartglobalizationsettings/getcharttitlename/
---
## ChartGlobalizationSettings.GetChartTitleName method

Obtiene el nombre del título del gráfico

```csharp
public virtual string GetChartTitleName()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetChartTitleNameDemo
    {
        public static void Run()
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

            // Demostrar el uso del método GetChartTitleName
            string chartTitleName = globalizationSettings.GetChartTitleName();
            Console.WriteLine("Chart Title Name: " + chartTitleName);

            // Guarda el libro de trabajo
            workbook.Save("ChartGlobalizationSettingsExample.xlsx");
        }
    }
}
```

### Ver también

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


