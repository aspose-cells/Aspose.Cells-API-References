---
title: "Series.HasSeriesLines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Verdadero si un gráfico de columnas apiladas o un gráfico de barras tiene líneas de series o si un gráfico Pie of Pie o Bar of Pie tiene líneas de conexión entre las dos secciones. Se aplica solo a gráficos de columnas apiladas, gráficos de barras, gráficos Pie of Pie o Bar of Pie"
type: docs
url: /es/net/aspose.cells.charts/series/hasserieslines/
---
## Series.HasSeriesLines property

True si un gráfico de columnas apiladas o de barras tiene líneas de serie o si un gráfico Pie of Pie o Bar of Pie tiene líneas de conexión entre las dos secciones. Se aplica solo a gráficos de columnas apiladas, gráficos de barras, gráficos Pie of Pie o Bar of Pie.

```csharp
public bool HasSeriesLines { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasSeriesLinesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Agregar un gráfico de columnas apiladas
            int chartIndex = worksheet.Charts.Add(ChartType.ColumnStacked, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar datos de la serie
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Acceder a la primera serie
            Series series = chart.NSeries[0];
            
            // Demostrar la propiedad HasSeriesLines
            series.HasSeriesLines = true; // Enable series lines
            
            // Guarda el libro de trabajo
            workbook.Save("SeriesHasSeriesLinesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


