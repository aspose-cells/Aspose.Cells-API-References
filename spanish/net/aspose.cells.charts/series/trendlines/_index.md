---
title: "Series.TrendLines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Devuelve todas las líneas de tendencia de esta serie"
type: docs
url: /es/net/aspose.cells.charts/series/trendlines/
---
## Series.TrendLines property

Devuelve todas las líneas de tendencia de esta serie.

```csharp
public TrendlineCollection TrendLines { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyTrendLinesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["A5"].PutValue(4);
            
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["B3"].PutValue(4);
            sheet.Cells["B4"].PutValue(8);
            sheet.Cells["B5"].PutValue(16);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Agregar una línea de tendencia exponencial a la primera serie y obtenerla por índice
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;

            // Guarda el libro de trabajo
            workbook.Save("TrendLinesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TrendlineCollection](../../trendlinecollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


