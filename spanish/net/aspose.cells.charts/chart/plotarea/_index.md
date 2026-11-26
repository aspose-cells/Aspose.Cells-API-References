---
title: "Chart.PlotArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Obtiene el área de trazado del gráfico que incluye las etiquetas de marcas del eje"
type: docs
url: /es/net/aspose.cells.charts/chart/plotarea/
---
## Chart.PlotArea property

Obtiene el área de trazado del gráfico que incluye las etiquetas de marcas del eje.

```csharp
public PlotArea PlotArea { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Personalizar el área de trazado
            chart.PlotArea.Area.FillFormat.FillType = FillType.Solid;
            chart.PlotArea.Area.FillFormat.SolidFill.Color = Color.LightBlue;
            chart.PlotArea.Border.Color = Color.Black;

            // Guarda el libro de trabajo
            workbook.Save("ChartPlotAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PlotArea](../../plotarea/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


