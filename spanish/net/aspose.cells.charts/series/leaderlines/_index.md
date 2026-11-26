---
title: "Series.LeaderLines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Representa líneas guía en un gráfico. Las líneas guía conectan las etiquetas de datos con los puntos de datos. Este objeto no es una colección; no hay un objeto que represente una sola línea guía"
type: docs
url: /es/net/aspose.cells.charts/series/leaderlines/
---
## Series.LeaderLines property

Representa líneas guía en un gráfico. Las líneas guía conectan las etiquetas de datos con los puntos de datos. Este objeto no es una colección; no hay un objeto que represente una sola línea guía.

```csharp
public Line LeaderLines { get; }
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
    public class SeriesPropertyLeaderLinesDemo
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

            // Agregar un gráfico de pastel
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurar etiquetas de datos
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowPercentage = true;
            series.DataLabels.Position = LabelPositionType.OutsideEnd;

            // Configurar líneas guía
            series.HasLeaderLines = true;
            series.LeaderLines.IsAuto = false;
            series.LeaderLines.Style = LineType.Dot;
            series.LeaderLines.WeightPt = 1.5;
            series.LeaderLines.Color = Color.Blue;

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertyLeaderLinesDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


