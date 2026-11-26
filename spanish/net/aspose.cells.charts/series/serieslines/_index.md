---
title: "Series.SeriesLines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Devuelve un objeto SeriesLines que representa las líneas de serie para un gráfico de barras apiladas o un gráfico de columnas apiladas. Se aplica solo a gráficos de barras apiladas y de columnas apiladas"
type: docs
url: /es/net/aspose.cells.charts/series/serieslines/
---
## Series.SeriesLines property

Devuelve un objeto SeriesLines que representa las líneas de serie para un gráfico de barras apiladas o un gráfico de columnas apiladas. Se aplica solo a gráficos de barras apiladas y columnas apiladas.

```csharp
public Line SeriesLines { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertySeriesLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["A5"].PutValue(4);
            
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar serie
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Personalizar líneas de serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.SeriesLines.Color = Color.Red;
            series.SeriesLines.Weight = Aspose.Cells.Drawing.WeightType.SingleLine;
            
            // Guarda el libro de trabajo
            workbook.Save("SeriesLinesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


