---
title: "Series.HasDropLines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Verdadero si el gráfico tiene líneas de caída. Se aplica solo a gráficos de líneas o de áreas"
type: docs
url: /es/net/aspose.cells.charts/series/hasdroplines/
---
## Series.HasDropLines property

True si el gráfico tiene líneas de caída. Se aplica solo a gráficos de líneas o de áreas.

```csharp
public bool HasDropLines { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasDropLinesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de líneas
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar datos de la serie
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener la primera serie
            Series series = chart.NSeries[0];

            // Demostrar la propiedad HasDropLines
            series.HasDropLines = true; // Enable drop lines
            series.Type = ChartType.Line; // Ensure it's a line chart for drop lines to be visible

            // Guarda el libro de trabajo
            workbook.Save("SeriesHasDropLinesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


