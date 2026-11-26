---
title: "Series.Points"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene la colección de puntos en una serie de un gráfico"
type: docs
url: /es/net/aspose.cells.charts/series/points/
---
## Series.Points property

Obtiene la colección de puntos en una serie de un gráfico.

```csharp
public ChartPointCollection Points { get; }
```

### Observaciones

Cuando el gráfico es Pie of Pie o Bar of Pie, el último punto es otro punto en la primera porción del pastel.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyPointsDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder a la primera serie y sus puntos
            Series series = chart.NSeries[0];
            foreach (ChartPoint point in series.Points)
            {
                // Agregar etiquetas de datos a cada punto
                point.DataLabels.ShowValue = true;
                point.DataLabels.ShowCellRange = true;
            }

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertyPointsDemo_Output.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPointCollection](../../chartpointcollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


